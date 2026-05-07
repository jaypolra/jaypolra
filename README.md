# Jay Polra

**Graduate Research Assistant @ CIVS, Purdue University Northwest**  
Computer Vision · Multimodal AI · Spatial Audio · Explainable AI · Industrial AI Safety

[![Portfolio](https://img.shields.io/badge/Portfolio-111827?style=flat&logo=googlechrome&logoColor=white)](https://www.datascienceportfol.io/jpolraa) [![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white)](https://github.com/jaypolra) [![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/jaypolra)

---

## About

I work on AI systems where the model is only part of the problem.

That problem shows up across computer vision, spatial audio, and vision-language models. Different domains, same question: what does it take for this to actually work outside the lab?

My background is in production systems before research, which means I've seen what happens when assumptions meet reality at scale.

---

## What I Work On

I'm drawn to problems where the assumptions a method makes are themselves worth questioning, because that's usually where the next research question is hiding.

In practice: a binaural audio model that assumes you have 3D geometry at inference time is a model with a fragile prerequisite. A safety system that assumes the camera sees everything is a system with a blind spot it doesn't know about. A vision-language model that produces confident captions is a model whose reasoning you can't verify until you build the tools to look inside it.

The work is about closing that gap, not just engineering around it, but understanding why it exists and what it reveals about the problem.

---

## Research & Projects

| Project | Venue / Status | What I was trying to solve |
|---|---|---|
| [geometry-grounded-nvas](https://github.com/jaypolra/geometry-grounded-nvas) | **CVPR Workshop 2026** | Prior audio-visual methods depend on Structure-from-Motion to build geometry: expensive, brittle with sparse frames, and unavailable at inference in many real scenes. Built a feed-forward pipeline using VGGT geometry encoding and a cross-attention decoder that routes on geometry but retrieves learned acoustic priors. No COLMAP, no target-view image required. |
| [ai-hazard-recognition](https://github.com/jaypolra/ai-hazard-recognition) | **AISTech 2026 submission** | The research question: can a camera-based safety system remain reliable when part of the environment is physically invisible to it? Detection alone fails here. A vehicle that disappears into a blind spot doesn't mean the zone is safe. Built entry-exit state tracking as a conservative safety heuristic: assume worst case until exit is confirmed by a boundary camera. |
| [vlm-hazard-reasoning](https://github.com/jaypolra/vlm-hazard-reasoning) | Research | Tested whether VLMs can reason about industrial hazards using domain-aware prompting, not just detect objects but explain why a scene is dangerous given the physical context of a melt shop. Explores the explainability gap that rule-based detection systems leave behind. |
| [vlm-explainer](https://github.com/jaypolra/vlm-explainer) | Research tool | BLIP generates fluent captions but gives no account of why. Built Grad-CAM token attribution, region masking, and perturbation testing to verify that highlighted regions actually caused the caption, not just correlated with it. Causality, not correlation, is the standard. |
| [candidate-matcher](https://github.com/jaypolra/candidate-matcher) | Applied NLP | Keyword overlap misses semantic alignment. A resume can match a job description on surface terms and still be irrelevant. Built semantic ranking using MiniLM embeddings and cosine similarity, with LLM-generated summaries that explain the match rather than just scoring it. |

---

## Before the Research

From 2023 to 2024, I worked as an SRE maintaining production systems across 11 global deployments: 25+ services, strict uptime requirements, real users on the other end.

It shaped one instinct that carried directly into research: you don't assume a system is working because nothing has broken yet. You build the thing that tells you *why* it's working, and whether that will still be true under different conditions, with different inputs, in an environment the system wasn't designed for.

That question follows me into every project.

---

## Tools I Work With

**Research & Modeling**  
`PyTorch` · `Hugging Face Transformers` · `OpenCV` · `Ultralytics YOLO` · `DeepSORT` · `BLIP` · `CLIP` · `VGGT`

**Applications & Infrastructure**  
`FastAPI` · `React` · `Streamlit` · `REST APIs` · `WebSockets` · `Terraform` · `Docker` · `Kubernetes`

**Languages**  
`Python` · `JavaScript` · `SQL` · `LaTeX` · `Git` · `CUDA`

---

*I try to build things that are honest about what they can and can't do.*
