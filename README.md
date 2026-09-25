# Riel St. Amand

**Senior full-stack engineer · Python / TypeScript · ML systems**

I turn model and infrastructure capabilities into reliable APIs, tools, and products, and then I measure whether they actually work instead of guessing.

I've spent six years shipping Python, React/TypeScript, and cloud systems end to end: a diagnostic ML platform that processed more than a million clinical tests, a text-to-SQL analytics product with its own eval harness, and a GRPO post-training pipeline that runs on one GPU. I'm currently an Engineer III at Smart Data, where I'm the sole engineer across several concurrent client engagements. I'm based in Kettering, OH.

---

## Building now

**[MockingBoard](https://mockingboard.app) + Songbird.** I founded MockingBoard and I'm its only engineer. It's a live-subscription product for the NFL Draft, fantasy, and stats, built as a TypeScript monorepo with Next.js, a Discord bot, Firebase, and Cloud Run. Songbird is its analytics layer: a routed, multi-model text-to-SQL system that writes schema-grounded SQL, charts the executed results, and builds answers only from the rows that came back. A custom eval harness and model judge score accuracy, latency, multi-step completion, and unsupported claims. In a prelaunch benchmark it beat two dedicated consumer NFL analytics assistants. It's now live on [draft](https://mockingboard.app), [fantasy](https://fantasy.mockingboard.app), and [stats](https://stats.mockingboard.app).

**[Kinewright](https://github.com/CanadaApollo6/Kinewright).** An open-source, agent-native video editor written in Rust that runs natively on Windows and Linux. It drives the agent CLI you already pay for (Claude Code, Codex, Cursor Agent, and others), so there are no API keys and no server. The agent's editing tools are generated from the same operation set the GUI uses, which means every agent edit is validated and undoable, just like a human's. Local Whisper transcription lets you edit by transcript down to the frame.

## Research

- **[tabular-reasoning-grpo](https://github.com/CanadaApollo6/tabular-reasoning-grpo).** An end-to-end GRPO/RLVR post-training system for reasoning over structured data. It uses seeded synthetic data, code-checked rewards, TRL + LoRA + vLLM, and multi-seed, multi-family evaluation. It improved a 1.7B model by **+14.2pp overall** and **+21.5pp on held-out real NFL data**, and the write-up covers the failure modes I hit along the way.
- **[psc-research](https://github.com/CanadaApollo6/psc-research).** Independent computational research into primary sclerosing cholangitis using public genetics, gene-expression data, and regulatory-sequence models (AlphaGenome). Every result ships with a frozen protocol, independent numerical verification, and a clean replay. Null results are reported as nulls. This one is personal: a member of my family lives with PSC.

## Open source

- **NVIDIA NeMo RL.** I diagnosed and fixed a GRPO checkpoint-resume bug that silently reset the reference policy and zeroed out KL regularization. The fix includes a single-GPU regression test plus logprob and weight-space provenance evidence. ([#3048](https://github.com/NVIDIA-NeMo/RL/pull/3048))
- **Omarchy plugins.**
  - [omarchy-task-manager](https://github.com/tcballard/omarchy-task-manager): cut GPU sampling cost from 12% to 3% of a core while the window is open, isolated the Qt test suites' runtime directory, and scoped the process list to the pages that show it.
  - [omarchy-retro-arcade](https://github.com/tcballard/omarchy-retro-arcade): fixed score-name entry in Circuit.
  - [omarchy-meeting-recorder](https://github.com/jankeesvw/omarchy-meeting-recorder): contributions in progress.
- **[Chartlite](https://github.com/chartlite/chartlite).** A lightweight TypeScript charting library built for content rather than dashboards, with reusable WCAG 2.1-accessible primitives.
- **[nflverse-ts](https://github.com/nflverse-ts).** I maintain the TypeScript port of the nflverse ecosystem ([nflreadts](https://github.com/nflverse-ts/nflreadts), [nflverse-types](https://github.com/nflverse-ts/nflverse-types)).

## Shipped in production

- **[Galen](https://github.com/CanadaApollo6/Galen-COVID19), Gravity Diagnostics.** I was the sole engineer on a COVID-19 diagnostic ML system. I built everything from instrument ingestion and 175K+ hand-labeled curves to five CNN-LSTM models running in the browser via TensorFlow.js, plus a React lab workstation. It processed **1M+ tests at 30K/day** and cut review time from ~15 minutes to under a second, with zero reported model corrections during parallel production validation.
- **CareSource MyLife.** A React/Remix SSR progressive web app serving 2M+ healthcare members across 5 states. It integrates 8 external systems, and its validation and UX work cut support tickets by about 90%.
- **Google Cloud, sales enablement.** I built the front end of an internal content delivery and onboarding platform for the Google Cloud Sales team.
- **Davey Tree, MyDavey customer portal.** An ASP.NET Core and React/TypeScript portal integrated with SAP Customer Data Cloud, Dynamics 365, and SAP bill pay. I fixed cross-domain SSO into bill pay and brought dev, QA, and production under Bicep infrastructure-as-code with OIDC deploys and least-privilege identities. I also automated dependency updates, nightly vulnerability scans, and environment promotion.
- **Schwarz Limited Partners, platform modernization.** I led security hardening alongside concurrent .NET and Angular upgrades, resolving 617 CVEs (153 in the first week). I'm now converting the single-tenant application to isolated per-client databases, which is projected to cut Azure spend by $25K–$40K a year.
- **Nationwide chatbot routing.** I rebuilt enterprise intent routing and raised accuracy from 64% to 94.8% (p < 0.01) on a UX-approved test set.
- **Document orchestration for Fortune 500 retailers.** A fault-tolerant, Redis-backed pipeline handling 800+ documents a day that cut processing time from 10 minutes to 30 seconds.

## Speaking & writing

- **Dayton AI Day 2026:** "Past the Paste"
- **KCDC 2022:** a four-hour ML Foundations workshop for 50+ engineers ([materials](https://github.com/CanadaApollo6/KCDC-2022-Materials))
- **HIMSS 2022**
- Technical writing at [rielstamand.dev](https://rielstamand.dev)

---

## Tools

**ML systems:** Python · PyTorch · Hugging Face · TRL · vLLM · GRPO / RLVR · LoRA · reward design · eval harnesses · LLM routing · text-to-SQL · TensorFlow / TF.js

**Backend & platform:** FastAPI · Node.js · .NET / C# · PostgreSQL · SQL Server · Redis · Docker · GCP · Azure

**Product & frontend:** React · TypeScript · Next.js · Remix · SSR & PWAs · data visualization · accessible UI (WCAG 2.1)

---

## Reach me

- Email: riel.stamand@gmail.com
- LinkedIn: [in/riel-st-amand](https://linkedin.com/in/riel-st-amand)
- Site: [rielstamand.dev](https://rielstamand.dev)
- X: [@RielStAmand](https://x.com/rielstamand)
