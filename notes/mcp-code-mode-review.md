# MCP, UTCP and Code Mode: review
Reviewed 30 October 2026. Source inspected: README.md, travel_server.py, demo1_classic.py, demo2_codemode.py and demo2_codemode.mjs in https://github.com/manojkanur/mcp-vs-code-mode . Static review only; demos not executed and paid model calls not made.

## Findings
UTCP is a separate tool-calling project, not an official MCP 2.0 release. Code Mode can wrap existing MCP tools. This demo uses the same MCP server for both approaches. Python is one implementation language; batching and filtering intermediate results cause the potential savings, not the language alone.

The server is real MCP software, but its business data is simulated: eight hardcoded cities, synthetic hourly weather, and a booking function that returns a fabricated reference without contacting an airline.

## Author-reported single runs
| Approach | Input tokens | Output tokens | Model calls | Tool calls | Time |
|---|---:|---:|---:|---:|---:|
| Classic | 16724 | 786 | 4 | 10 | 9.2s |
| TypeScript | 6709 | 522 | 3 | 10 | 6.3s |
| Python | 4268 | 531 | 2 | 10 | 5.7s |
Input savings are about 60% and 74%. These are not reproduced measurements or a guarantee. The different prompts and generated execution plans also affect results; the Python language itself has not been isolated as the cause. The classic client can receive several tool calls in a model response, so the example does not establish that MCP inherently requires one model turn per tool.

## Implementation limits
Both Code Mode clients put all generated tool interfaces into the model prompt; one visible tool does not mean zero tool-description overhead. They also return result plus logs, so verbose logs can erode savings. Both retain conversation history. The model loop has no explicit maximum number of rounds or total token budget. The Python demo patches private library methods and adds four compatibility fixes. Separate environments are required because the classic demo pins mcp==2.3.0 while utcp-mcp requires mcp<2. RestrictedPython should not be treated as a strong security boundary. Setup examples use Unix paths and export; Windows needs adapted instructions.

## Practical token policy
1. Fetch only relevant files, fields and rows; avoid printing entire repositories or raw API payloads.
2. Batch independent reads, then filter, aggregate and deduplicate in code before returning a short result.
3. Discover only relevant tools where supported. Keep useful identifiers, citations and error counts.
4. Store large intermediate results outside model context; retrieve targeted portions when needed.
5. Set maximum rounds, execution time, output size and spending limits. Keep approval boundaries for real-world writes.
6. Benchmark the same tasks and model across repeated runs. Record input/output and cached tokens, actual cost, latency, correctness, retries and failures. A cheap wrong answer is not an improvement.
7. Use ordinary direct tool calls for simple tasks; adopt Code Mode where multi-step data processing justifies its setup overhead.

Example: read 100 job listings, filter and deduplicate in code, return the best 10 with links and reasons rather than all raw listings. Keep applications or messages as a separate user-approved step.

## Supplied resources
- Repository: https://github.com/manojkanur/mcp-vs-code-mode
- Your fork: https://github.com/vi14cute/mcp-vs-code-mode
- Claude artifact: https://claude.ai/artifact/GXqK2CGJi3Qj5STPMj3eEh (web reader could not access; content unverified).
- Community/interest page: https://becomeaneagle.edgeone.app/?form=form_manoj-interest-whatsapp (web reader could not access; content unverified; no form submitted).
- Creator/consulting profile: https://topmate.io/the_ai_dude (profile accessible; no booking or message made).
- Primary Code Mode project: https://github.com/universal-tool-calling-protocol/code-mode
