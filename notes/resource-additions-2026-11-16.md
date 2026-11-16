# Resource additions - 16 November 2026

This batch covers **all 9 directly supplied web resources and both PDFs**. Tracking parameters were removed. Repository copies preserve their upstream authors and licenses. Notes describe reviewed sources; advertised performance, test counts and employment outcomes were not independently reproduced.

## New repository copies

| Repository copy | Original | Practical use | Laptop fit and status |
| --- | --- | --- | --- |
| [skills / StageShow](https://github.com/vi14cute/skills/tree/main/stageshow) | [benjitaylor/skills](https://github.com/benjitaylor/skills) | React product illustrations, feature cards and animated UI demonstrations for a portfolio or app launch | StageShow skill installed locally. This creates demonstrations, not the working application behind them. |
| [gpu-unlock](https://github.com/vi14cute/gpu-unlock) | [Zagitta/gpu-unlock](https://github.com/Zagitta/gpu-unlock) | Advanced NVIDIA tensor-performance research | Reference only. Upstream targets supported NVIDIA RTX cards on Linux; the current Intel UHD Windows laptop is incompatible. Not installed or benchmarked. |
| [ECC](https://github.com/vi14cute/ECC) | [affaan-m/ECC](https://github.com/affaan-m/ECC) | Study planning, testing, code review, context management and reusable agent workflows | Saved for selective study. Its hooks, plugins and agent configuration were not installed. More agents do not automatically improve results or save tokens. |
| [beginner-local-rag-system](https://github.com/vi14cute/beginner-local-rag-system) | [jamwithai/beginner-local-rag-system](https://github.com/jamwithai/beginner-local-rag-system) | Learn document retrieval and answers grounded in retrieved passages | OpenSearch, embeddings and a local model share memory. Start with a small dataset; reliable speed on an 8GB laptop has not been established. |
| [production-agentic-rag-course](https://github.com/vi14cute/production-agentic-rag-course) | [jamwithai/production-agentic-rag-course](https://github.com/jamwithai/production-agentic-rag-course) | Build an arXiv research assistant through ingestion, keyword search, vectors, monitoring and agents | README specifies Docker, Python 3.12+, 8GB+ RAM and 20GB+ storage. An 8GB Windows system is at the listed minimum, not a guarantee of comfortable operation. Study one component at a time. |
| [observable-job-agent](https://github.com/vi14cute/observable-job-agent) | [jamwithai/observable-job-agent](https://github.com/jamwithai/observable-job-agent) | Learn job matching, evidence-linked resume tailoring, tracing and evaluation | Start with offline fixtures and tests. Agent calls need an LLM provider or local model; tracing and optional voice have separate setup. No provider keys or paid services configured. |
| [career-ops](https://github.com/vi14cute/career-ops) | [career-ops-hq/career-ops](https://github.com/career-ops-hq/career-ops) | Organize job opportunities, compare roles and prepare application drafts | Discovered through the supplied official website. CLI-based workflow; provider cost and data handling depend on the chosen AI engine. Not installed. Human reviews and submits applications. |

The three Jam with AI repositories have MIT licenses. StageShow is MIT with separate third-party asset notices. ECC and Career Ops identify as MIT. GPU Unlock identifies as GPL-2.0. Review the actual license and dependency/asset notices before redistribution.

## Complete input coverage

| # | Supplied item | What was retained / review status |
| --- | --- | --- |
| 1 | [StageShow skill repository](https://github.com/benjitaylor/skills/tree/main/stageshow) | Fork, practical-use note and local skill installation. Main skill instructions read; dependencies and demo scripts not run. |
| 2 | [GPU Unlock](https://github.com/Zagitta/gpu-unlock) | Fork and hardware incompatibility note. README reviewed; speed claims remain upstream claims. |
| 3 | [How I turned myself 3D](https://app.notion.com/p/How-I-turned-myself-3D-40771fb1e01c81c9bc60e952c2900055) | Guide accessible in Chrome. Create a multi-view character reference, correct it incrementally, and reuse the final reference for scenes. Some embedded prompt blocks did not load; this is a workflow summary, not a full archive. |
| 4 | [Shared Google Drive folder](https://drive.google.com/drive/folders/1eX5CKIXwL62iWnvQc2tINo-6Oz4xzJ7S) | Link preserved. Both the connected reader and Chrome returned 404/not found. Contents unknown; a corrected or accessible link is needed to inventory them. |
| 5 | [Higgsfield Katana / ChatGPT page](https://higgsfield.ai/start/katana?tab=chatgpt) | Link preserved with functional tab parameter. Chrome loaded Higgsfield navigation, but the main content stayed loading. Katana-specific instructions and claims unverified. No subscription or generation started. |
| 6 | [Career Ops](https://career-ops.org/) | Official site reviewed; linked source repository forked. Useful for job-search organization and application preparation. Cloud AI provider calls may still send data off-device even when the project stores files locally. |
| 7 | [ECC](https://github.com/affaan-m/ECC) | Fork and selective-workflow study note; README reviewed. |
| 8 | [2026 AI Engineer Roadmap](https://docs.google.com/document/d/12WgyLe41H6P5Hn7gK2u3vCcVx6vTQLbURTBSmyY9jIQ/edit) | Spaces in the supplied URL removed; title and document contents verified. It contains the presentation and explainer links below. |
| 9 | [n8n's BIGGEST AI Update Yet?! (Tamil)](https://www.youtube.com/watch?v=xgm5mtvhfbo) | Title and channel, The AI Dude - Tamil, verified. Saved for automation study; full video/transcript not reviewed, so feature claims are not summarized as facts. |
| 10 | build-3-repo-guide-jamwithai.pdf | All 6 pages inspected. Three unique GitHub projects retained above; companion links listed below. PDF commands were treated as reference text, not executed. |
| 11 | Machine Learning Repos (1).pdf | Its single page lists the same five existing forks below. File SHA-256 exactly matches the previously supplied Machine Learning Repos.pdf. No duplicate forks created. |

## PDF coverage and companion references

### Build guide: 6 pages

- Pages 1-2: overview and comparison of the same three repositories.
- Page 3: Beginner Local RAG System and two companion articles:
  - [Local RAG - Part 1](https://jamwithai.substack.com/p/build-a-local-llm-based-rag-system)
  - [Local RAG - Part 2](https://jamwithai.substack.com/p/build-a-local-llm-based-rag-system-628)
- Page 4: Production Agentic RAG Course.
- Page 5: Observable Job Agent.
- Page 6: suggested progression and creator references:
  - [Jam with AI newsletter](https://jamwithai.substack.com)
  - [Jam with AI website](https://jamwithai.dev)
  - [Jam with AI YouTube](https://www.youtube.com/@jam-with-ai)
  - [Jam with AI GitHub](https://github.com/jamwithai)

Companion references are preserved as links, not claimed to have been fully reviewed. The source PDF dates its GitHub statistics to 3 November 2026; those numbers are not used as current quality or performance evidence. Some copied commands contain layout/extraction artifacts. Follow the current upstream README rather than pasting extracted PDF commands.

### Machine-learning PDF: 5 existing forks, verified present

1. [ML-For-Beginners](https://github.com/vi14cute/ML-For-Beginners) - [Microsoft original](https://github.com/microsoft/ML-For-Beginners): regression, classification and clustering.
2. [handson-mlp](https://github.com/vi14cute/handson-mlp) - [Ageron original](https://github.com/ageron/handson-mlp): hands-on algorithms and notebooks.
3. [fastbook](https://github.com/vi14cute/fastbook) - [fastai original](https://github.com/fastai/fastbook): practical deep learning. Book text and code have different reuse terms; preserve both.
4. [pytorch-deep-learning](https://github.com/vi14cute/pytorch-deep-learning) - [Daniel Bourke original](https://github.com/mrdbourke/pytorch-deep-learning): tensors, networks and training.
5. [mlops-zoomcamp](https://github.com/vi14cute/mlops-zoomcamp) - [DataTalksClub original](https://github.com/DataTalksClub/mlops-zoomcamp): experiment tracking, deployment and monitoring.

Each repository link appears twice in the PDF annotations; each is catalogued once.

### Links inside the roadmap document

- [Roadmap presentation](https://drive.google.com/file/d/1omS_swcvuZkJgV2diDpXmPV8BZL-8gh0/view)
- [Roadmap video explainer](https://youtu.be/XpIlC6hU0ns)

These two destinations were found in the verified document and preserved; their complete contents were not reviewed.

## Use this collection deliberately

Suggested starting priorities, based on the sources reviewed and the current i3/8GB laptop:

1. **Practical career help:** inspect Career Ops using one public job description and a synthetic resume before introducing personal documents.
2. **Portfolio engineering:** study Observable Job Agent's evidence links, deterministic validation and per-run cost tracking. Build an original small feature and measure it; a fork alone is not original work.
3. **Document-based application work:** learn retrieval with the beginner RAG project. Borrow the ideas for ClearStep, keeping official citations, unknown states and human review.
4. **Presentation:** use StageShow after there is a working application, to create an honest product walkthrough. Label simulated UI as a demo.
5. **Later:** study the production RAG stack and choose individual ECC practices once a smaller project works. GPU Unlock stays a hardware reference.

For token efficiency: retrieve only relevant passages, cache unchanged results, use ordinary code for exact checks, cap retries and record actual input/output tokens and costs. Compare quality against a baseline before claiming savings.

## Preservation and verification

- This update stores source-code forks plus original summaries and clean reference links. It does not upload complete third-party PDFs, private documents, personal resumes, API keys or generated media.
- All branches were requested when creating each new fork. Branch/tag counts are point-in-time observations, not promises of automatic synchronization.
- A GitHub fork copies repository source/history, not every upstream issue, release binary or service setting.
- Only StageShow's skill files were installed. Installing the skill does not install its React dependencies, build its examples, or demonstrate that every helper works on Windows.
- The installed SKILL.md reports StageShow 1.1.1. It will be available to Codex on the next turn.
- Saved links can expire or change. Recheck access and current requirements when starting a project.
