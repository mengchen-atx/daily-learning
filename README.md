
## 2026-03-06 Learning Log
Deep Learning:
Learned the fundamental loss function in linear regression and optimization:

1. **Training Loss (Mean Squared Error)**:
```math
\ell(\mathbf{X}, \mathbf{y}, \mathbf{w}, b) = \frac{1}{2n} \sum_{i=1}^{n} (y_i - \langle \mathbf{x}_i, \mathbf{w} \rangle - b)^2 = \frac{1}{2n} \| \mathbf{y} - \mathbf{X}\mathbf{w} - b \|^2
```

This formula represents the Mean Squared Error (MSE) loss function, which measures the average squared difference between predicted values and actual labels. The vectorized form on the right side enables efficient batch computation.

2. **Optimal Parameter Learning**:

```math
\mathbf{w}^*, b^* = \arg\min_{\mathbf{w},b} \ell(\mathbf{X}, \mathbf{y}, \mathbf{w}, b)
```

This formula defines the optimization objective: find the weight vector $\mathbf{w}^*$ and bias $b^*$ that minimize the training loss. This is the core principle behind parameter learning in linear regression models.

3. **Gradient Descent Update Rule**:

```math
\mathbf{w}_t = \mathbf{w}_{t-1} - \eta \frac{\partial \ell}{\partial \mathbf{w}_{t-1}}
```

This formula represents the gradient descent optimization algorithm, where $\mathbf{w}_t$ is the updated weight vector at iteration $t$, $\eta$ is the learning rate (step size), and $\frac{\partial \ell}{\partial \mathbf{w}_{t-1}}$ is the gradient of the loss function with respect to the weights. This iterative process gradually minimizes the loss by moving in the direction of steepest descent.

## 2026-03-05 Learning Log
Deep Learning:
Learned matrix calculation, linear algebra

## 2026-03-04 Learning Log
Deep Learning:
Learned data pre-processing

## 2026-03-03 Learning Log
Deep Learning:
Learned the basic data manipulation, broadcasting mechanism

## 2026-03-02 Learning Log
Deep Learning:
Learned the environment. Installed jupyter,d2l,torch,torchvision.

## 2026-03-01 Learning Log
Rosalind

## 2026-02-28 Learning Log
Rosalind

## 2026-02-27 Learning Log
Skill-RL
Deepened understanding of the project architecture by mapping the three core contributions from the paper to the actual codebase:

1. **Skill Generation (Distilling Experience)**: The `skill_generation/` module implements the distillation process that converts raw trajectories into structured skills. This is where the teacher model's guidance transforms lengthy experience sequences into concise, actionable knowledge.

2. **SkillBank (Skill Library)**: Located in `agent_system/memory/`, this module manages the persistent storage and organization of the skill library. It serves as the central knowledge repository that supports both skill retrieval during inference and skill updates during the co-evolution process.

3. **RL Training (Policy Evolution)**: The combination of `gigpo/`, `verl/`, and `recipe/` modules handles the reinforcement learning pipeline. This where the skill library and policy are jointly optimized through feedback from failed trajectories and new skill proposals.

  ---
  项目整体架构（从论文的 3 个核心贡献对应到代码）

  论文概念                    对应代码位置
  ─────────────────────────────────────────────────────
  ① Skill 生成（蒸馏经验）   skill_generation/
  ② SkillBank（技能库）       agent_system/memory/
  ③ RL 训练（策略进化）       gigpo/ + verl/ + recipe/




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