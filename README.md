#  Reinforcement Pre-Training (RPT)

This repository contains a lightweight prototype of Microsoft's **Reinforcement Pre-Training (RPT)** paper, adapted to run on a local M1 Mac using a distilled GPT-2 model.

We simulate the RPT idea by reframing **next-token prediction** as a reward-based task — rewarding the model for correctly predicting each next token.

## 📌 What’s Inside

-  Custom dataset loader (JSONL format with prompt-completion pairs)
-  Reward-weighted training loop (token-wise correctness → reward)
-  DistilGPT2-based prototype (optimized for low-resource Macs)
-  No reliance on Hugging Face `datasets` cache (to avoid local FS bugs)
-  Training logs + comments for clarity

##  Core Concept

> **Reinforcement Pre-Training (RPT)** reframes next-token prediction as a *reasoning task* trained via Reinforcement Learning.  
> Models receive direct, verifiable rewards for correct predictions — encouraging internal reasoning and reducing reward hacking.

