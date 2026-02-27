## 2026-02-26 Learning Log
Skill-RL  
Two core mechanisms:
1. High-level skill abstraction： By leveraging a powerful teacher model, the lengthy and noisy original success and failure trajectories are distilled and refined into a structured skill library (SKILLBANK) that encompasses general strategies and specialized techniques. This approach replaces rote memorization with highly condensed and reusable behavioral principles, achieving a 10-20 times reduction in Token compression while significantly enhancing the efficiency of intelligent search and reasoning.

2. Co-evolving library: By using recursive skill evolution. Low success rate will collect failure trajectories and utilize the teacher model to propose new skills or modify the ineffective old skills.

## 2026-02-25 Learning Log
Skill-RL  
The most fundamental and core formula in deep learning and natural language processing (NLP). Its full name is the objective function of Supervised Fine-Tuning (SFT, supervised fine-tuning).

```math
\theta_{\text{sft}} = \arg\min_{\theta} \mathcal{L}_{\mathrm{CE}}(D_{\mathrm{SFT}};\theta)
```
Meaning: find parameters θ minimizing cross-entropy loss on SFT dataset.

## 2026-02-24 Learning Log
Skill-RL
1. Transform redundant trajectories into concise and actionable knowledge.
2. Put distilled experiences into skill library S (classified general and task-specific expertise)
3. Use RL to refine the skill Library S and agent's policy.

## 2026-02-23 Learning Log
Learned how to install agent skills (planning-with-files) for claude code. 

## 2026-02-22 Learning Log
Installed Pixel Agents in VS Code by cloning the repository locally. Since the extension's required version was incompatible, I manually adjusted the engines field in package.json to match my current VS Code version and successfully run it from source.

## 2026-02-21 Learning Log
Learned the difference between MCP and agent skills.

## 2026-02-20 Learning Log
Enhanced the performance and usability of the mini-program.

## 2026-02-19 Learning Log
Developed a mini-program for second-hand buying and selling.

## 2026-02-18 Learning Log
Started exploring IsoNet2 on GitHub. Learned basic Git operations (commit, push) and how the GitHub contribution graph works.

## 2026-02-17 Learning Log
Set up Git clone and configured VS Code shortcuts.