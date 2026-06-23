# Riel St. Amand

**Machine learning engineer working on reinforcement learning and post-training for language models.**

I work on teaching models to reason — and on the harder, less glamorous problem of proving they actually got better. My current focus is verifiable-reward RL (GRPO / RLVR), post-training on a single-GPU budget, and evaluation rigorous enough to tell a real gain from a lucky seed.

Based in Dayton, OH. Currently an Engineer III at Smart Data; previously built production ML in clinical diagnostics.

---

## What I'm working on

**A GRPO pipeline that teaches a small language model to reason over structured data — on one GPU.**
Verifiable rewards (a correctness check plus a format signal), TRL's `GRPOTrainer` with LoRA, and vLLM-accelerated rollouts. The part I care most about is the evaluation: accuracy broken out by task type, scored against a naive best-constant floor, with Wilson confidence intervals and a paired McNemar test — plus a written record of the failure modes I hit (KL drift, reward-gaming, the rollout bottleneck) and how I diagnosed each one.

[Code and write-up →](https://github.com/CanadaApollo6/gridiron-grpo)

## Research

Two papers in preparation / under submission:

- **Evaluating reasoning models against deductive ground truth.** A setting where the correct answer is fixed by construction, so you can measure *how* a model fails — not just whether — and watch its recovery as you give it more to work with. *(in submission)*
- **When does verifiable-reward RL actually help?** An empirical study of GRPO / RLVR on structured, tabular reasoning across model families: where the gains are real, where they're seed noise, and what predicts the difference. *(in preparation)*

## Production ML (background)

Before the research turn, I built and shipped ML in clinical diagnostics:

- A production COVID-19 diagnostic system at Gravity Diagnostics — an ensemble of CNN-LSTM models that processed **1M+ tests** at roughly **30,000 per day**, validated to match human lab technicians, cutting turnaround from about 15 minutes to under a second.

I also led the AI & Machine Learning workshop at Kansas City Developer Conference (KCDC) 2022, and I write and speak on agentic AI and small-model reasoning.

---

## Tools

**RL / post-training:** PyTorch · TRL · vLLM · GRPO / RLVR · LoRA / PEFT · reward design · evaluation & failure-mode analysis

**Also:** Python · TypeScript · C# · SQL · FastAPI · TensorFlow

---

## Reach me

- Email: riel.stamand@gmail.com
- LinkedIn: [in/riel-st-amand](https://linkedin.com/in/riel-st-amand)
- Site: [rielstamand.dev](https://rielstamand.dev)
- X: ‹your handle›
