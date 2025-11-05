---
layout: page
title: Home
---

# DSC 180A — Methodology Assignment 4 (Task 2)

**Name & Email**  
Banff Jiang — bxjiang@ucsd.edu

**Section & Mentor**  
Section: A10
Mentor: Alex Warstadt

---

**What is the most interesting topic covered in your domain this quarter?**  
The most interesting topic for me has been how **model architecture and training curricula fundamentally impact sample efficiency**. In BabyLM, we restrict data to ~100M tokens, so we can’t rely on brute-force scaling. That forces us to think deeply about design choices like pre-layer norm architectures, masking strategies, warmup schedules, and curriculum pacing. It’s been fascinating seeing how small changes can drastically improve learning under low-resource conditions.

**Describe a potential investigation you would like to pursue for your Quarter 2 Project.**  
I would like to explore **LTG-BERT Ablations** to disentangle which architectural modifications actually matter in data-limited training. Rather than treating the final leaderboard score as a black box, I’d run controlled ablation studies that isolate the effect of: (1) pre-layer normalization, (2) weight sharing, and (3) tokenizer vocabulary size. The goal is to better understand what yields “free performance gains” when scaling **down** instead of up.

**What is a potential change you’d make to the approach taken in your current Quarter 1 Project?**  
Right now, our Quarter 1 work is mainly **hands-on training using provided repositories**, with most of the engineering decisions already implemented for us. We primarily focus on running models, tracking perplexity, and comparing different checkpoints rather than deeply modifying model internals. A change I would make is to allocate more time for **custom experimentation**, for example, modifying masking strategies, adjusting tokenizer configuration, or implementing small architectural tweaks. This would help us move beyond simply executing predefined scripts toward a better understanding of *why* certain design choices reduce perplexity under limited-data constraints

**What other techniques would you be interested in using in your project?**  
I want to explore **minimal multimodal integration** , revisiting the idea that adding lightweight vision grounding could improve semantic generalization without large architecture changes. I’m also interested in lightweight evaluation improvements like probing tasks