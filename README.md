# V-skip

<div align="center">

[![arXiv](https://img.shields.io/badge/arXiv-2601.13879-b31b1b.svg)](https://arxiv.org/pdf/2601.13879)
[![Project Page](https://img.shields.io/badge/Project-Page-green)](https://dongxu-zhang.github.io/v-skip.github.io/)
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)

**V-Skip: Efficient Multimodal Reasoning via Dual-Path Anchoring**
<br>
[Dongxu Zhang](https://dongxu-zhang.github.io/)<sup>1,*</sup>, [Yiding Sun](https://github.com/Issac-Sun)<sup>1,*</sup>, [Cheng Tan](https://chengtan9907.github.io/)<sup>3</sup>, [Wenbiao Yan](#)<sup>4</sup>, [Ning Yang](http://ningyangcasia.cn/)<sup>2,†</sup>, [Jihua Zhu](https://gr.xjtu.edu.cn/web/zhujh)<sup>1,†</sup>, [Haijun Zhang](https://scce.ustb.edu.cn/shiziduiwu/jiaoshixinxi/2018-04-13/100.html)<sup>5</sup>

<sup>1</sup>Xi'an Jiaotong University, <sup>2</sup>CASIA, <sup>3</sup>Shanghai AI Laboratory, <sup>4</sup>HITSZ, <sup>5</sup>USTB
</div>

---

## 🚀 Introduction

This repository contains the official implementation (and project page source) for the paper **"Chain-of-Thought Compression Should Not Be Blind: V-Skip for Efficient Multimodal Reasoning via Dual-Path Anchoring"**.

**V-Skip** is a novel token pruning framework designed for Multimodal Large Language Models (MLLMs). It solves the **"Visual Amnesia"** problem found in standard text-centric compression methods. By employing a dual-path gating mechanism (Linguistic Surprisal + Visual Attention Flow), V-Skip preserves visually salient tokens while reducing latency.

![V-Skip Teaser](./static/images/fig1.png)
*Figure 1: Comparison of compression paradigms. V-Skip successfully rescues visual anchors (e.g., "red") that are blindly pruned by text-only methods.*

## 📈 Key Results
- **Speedup:** Achieves **2.9x** inference speedup on Qwen2-VL.
- **Accuracy:** Outperforms baselines by over **30%** on the DocVQA benchmark.
- **Robustness:** Effectively prevents object hallucination caused by over-pruning.

## 🛠️ Usage
