# 🧠 LifeDialBench: Evaluating Memory Capability in Continuous Lifelog Scenarios





> **Evaluating Memory Capability in Continuous Lifelog Scenario**  
> Jianjie Zheng, Zhichen Liu, Zhanyu Shen, Jingxiang Qu, Guanhua Chen†, Yile Wang, Yang Xu, Yang Liu, Sijie Cheng†  
> Southern University of Science and Technology · RayNeo.AI · Tsinghua University · Shenzhen University · Shanghai Jiao Tong University  
> ( Equal contribution. † Corresponding authors.)

---

## 🚧 Coming Soon

> The **LifeDialBench dataset** (EgoMem & LifeMem subsets), evaluation scripts, and baseline implementations will be released upon paper acceptance.  
> Please ⭐ **star this repo** to stay updated!

---

## 📌 Overview

Wearable devices such as smart glasses (e.g., Ray-Ban Meta, RayNeo V3/X3) and always-on recording machines enable continuous lifelogging of ambient conversations. This creates a fundamentally new challenge for memory systems — one that existing benchmarks, which focus on one-on-one chat or human-AI interactions, are ill-equipped to address.

We introduce **LifeDialBench**, a novel benchmark designed to evaluate long-term memory systems in realistic, continuous dialogue lifelog scenarios.

  
*Figure 1: Comparison between the microphone-always-on lifelog scenario and the conventional on-demand human-AI chatting scenario.*  
[Download PDF]

---

## ✨ Key Features

- **Two Complementary Subsets**
  - 🎥 **EgoMem** — Built on real-world egocentric videos (derived from the EgoLife dataset), capturing naturalistic multi-party conversations in-the-wild.
  - 🏘️ **LifeMem** — Constructed from a simulated virtual community, providing rich, dense, and controllable long-term dialogue scenarios.
- **Hierarchical Synthesis Framework** — A principled pipeline for curating high-quality, temporally consistent dialogue lifelogs with human-in-the-loop review.
- **Online Evaluation Protocol** — A novel evaluation paradigm that strictly adheres to temporal causality, preventing temporal leakage and ensuring systems are assessed in a realistic streaming fashion.

  
*Figure 2: Overview of the LifeDialBench benchmark construction framework and online evaluation protocol.*  
[Download PDF]

---

## 🔍 Key Finding

> *Current sophisticated memory systems fail to outperform a simple RAG-based baseline.*

Our experiments reveal a **counterintuitive result**: over-designed memory structures and lossy compression strategies actively **hurt** performance in lifelog scenarios. This highlights the critical importance of **high-fidelity context preservation**.

---

## 📂 Dataset

> 🚧 **Coming Soon** — will be released upon paper acceptance.

The benchmark will include:


| Subset      | Source                                | Setting                                |
| ----------- | ------------------------------------- | -------------------------------------- |
| **EgoMem**  | Real-world egocentric video (EgoLife) | In-the-wild, multi-party conversations |
| **LifeMem** | Simulated virtual community           | Controlled, long-horizon lifelog       |


---

## 🚀 Getting Started

> 🚧 Code and evaluation scripts are coming soon.

```bash
# Clone the repository
git clone https://github.com/qys77714/LifeDialBench.git
cd LifeDialBench
```

Requirements and setup instructions will be provided upon release.

---

## 📊 Evaluation

We provide an **Online Evaluation Protocol** that simulates a streaming, temporally-ordered inference setting — in contrast to traditional offline protocols which risk temporal leakage.

Evaluation scripts and detailed instructions will be released alongside the dataset.

---

## 📖 Citation

If you find LifeDialBench useful in your research, please cite our paper:

```bibtex
@article{zheng2026lifedialbench,
  title     = {Evaluating Memory Capability in Continuous Lifelog Scenario},
  author    = {Zheng, Jianjie and Liu, Zhichen and Shen, Zhanyu and Qu, Jingxiang and
               Chen, Guanhua and Wang, Yile and Xu, Yang and Liu, Yang and Cheng, Sijie},
  journal   = {arXiv preprint},
  year      = {2026},
  url       = {[YOUR_ARXIV_LINK]}
}
```

