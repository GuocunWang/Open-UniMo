# Open-UniMo: Towards Unified Motion-Language Understanding and Generation in the Open World

<p align="center">
  <a href="https://github.com/GuocunWang/Open-UniMo">
    <img src="https://img.shields.io/badge/Code-GitHub-black.svg" alt="GitHub">
  </a>
  <a href="https://github.com/GuocunWang/UniMo">
    <img src="https://img.shields.io/badge/Previous-UniMo-blue.svg" alt="UniMo">
  </a>
</p>

<p align="center">
  <b>
    Guocun Wang<sup>1*</sup>,
    Kenkun Liu<sup>2*</sup>,
    Guorui Song<sup>1*</sup>,
    Jing Lin<sup>3</sup>,
    Zhe Huang<sup>1</sup>,
    Luyuan Zhang<sup>1</sup>,
    Dake Zhong<sup>1</sup>,
    Choo Sin Wai<sup>1</sup>,<br>
    Xiaoguang Han<sup>2</sup>,
    Haoqian Wang<sup>1†</sup>
  </b>
  <br>
  <sup>1</sup>Tsinghua University,
  <sup>2</sup>The Chinese University of Hong Kong, Shenzhen,
  <sup>3</sup>Nanyang Technological University
  <br>
  <sup>*</sup>Equal contribution &nbsp;&nbsp;
  <sup>†</sup>Corresponding author
</p>

---
<img width="7999" height="3353" alt="teaser" src="https://github.com/user-attachments/assets/a845be9f-4851-4347-9631-aa13448ea1a3" />

## 🔥 News

- Open-UniMo is released as an extension of our previous work [UniMo](https://github.com/GuocunWang/UniMo).

---

## 📖 Introduction

**Open-UniMo** is a unified **Large Motion-Language Model (LMLM)** for open-world human motion generation and understanding.

Existing motion-language models often treat motion as an auxiliary modality of a language model, resulting in text-dominated representations and limited cross-modal interaction. Moreover, autoregressive next-token prediction can accumulate errors over long motion sequences.

Open-UniMo addresses these challenges by:

- 🚀 **Scaling unified motion-language modeling to million-scale open-world data.**
- 🧩 **Extending the Qwen vocabulary with 64K motion tokens**, treating motion as a first-class modality in a unified token space.
- 🧠 Introducing **CoT** as an intermediate representation between language semantics and motion dynamics.
- 🎯 Adopting a two-stage **SFT → GRPO** training pipeline to improve cross-modal semantic alignment and mitigate cumulative errors in autoregressive motion generation.
- 📊 Introducing **Open-MoBench**, a VLM-guided benchmark that jointly evaluates Text-to-Motion generation, Motion-to-Text understanding, and bidirectional consistency.

Open-UniMo achieves state-of-the-art performance on both conventional metrics and Open-MoBench. Our experiments further reveal that generation and understanding are not isolated abilities: coupling M2T understanding with the learnable T2M generation path produces stronger cross-modal representations, showing that **generation can facilitate understanding in AR-based motion-language models**.
