# Awesome Agentic Time Series

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
[![Papers](https://img.shields.io/badge/Papers-200%2B-blue.svg)](#contents)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](#contributing)

A curated paper list for **Agentic Time Series**, covering the evolution from time series foundation models and LLM4TS to temporal reasoning, memory, world models, reliability, and fully agentic time series systems.

> Associated survey: **The Landscape of Agentic Time Series Systems: Paradigms, Architectures, Reliability, and Frontiers**.

## News

- **2026-06** Initial release of `Awesome-Agentic-Time-Series` .
- Contributions are welcome. If a relevant paper is missing or misclassified, please open an issue or submit a pull request.

## Contents

- [Surveys and Position Papers](#surveys-and-position-papers)
- [Benchmarks and Datasets](#benchmarks-and-datasets)
- [Time Series Foundation Models](#time-series-foundation-models)
- [LLM4TS: Translation and Alignment](#llm4ts-translation-and-alignment)
- [LLM4TS: Temporal Reasoning](#llm4ts-temporal-reasoning)
- [Agentic Time Series Systems](#agentic-time-series-systems)
  - [Perception Agents](#perception-agents)
  - [Reasoning Agents](#reasoning-agents)
  - [Planning & Action Agents](#planning--action-agents)
  - [Memory & Knowledge Agents](#memory--knowledge-agents)
  - [World-Model & Data Agents](#world-model--data-agents)
- [Reliability, Safety and Trustworthiness](#reliability-safety-and-trustworthiness)
- [Contributing](#contributing)
- [Citation](#citation)

## Taxonomy

This repository follows the taxonomy used in the survey:

- **Benchmarks and datasets** evaluate forecasting, reasoning, multimodal understanding, ML engineering, tool use, and decision safety.
- **Time series foundation models** learn general-purpose temporal representations and support zero/few-shot forecasting or other downstream tasks.
- **LLM4TS** includes translator-style methods for aligning time series with language/multimodal spaces and reasoner-style methods for explicit temporal reasoning.
- **Agentic time series systems** are organized by five capability layers: perception, reasoning, planning and action, memory and knowledge, and world-model/data-agent capabilities.
- **Reliability and trustworthiness** cut across all categories, covering forecasting quality, reasoning correctness, tool-use reliability, hallucination and grounding, decision safety, auditability, and reproducibility.


## Surveys and Position Papers

### 2024

- [Large Language Models for Time Series: A Survey](https://arxiv.org/pdf/2402.01801) (2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2402.01801)  
  *2024 · Forecasting, Classification, Anomaly Detection, Imputation, QA-Reasoning · ToolUse*

### 2025

- [A Survey of Reasoning and Agentic Systems in Time Series with Large Language Models](https://arxiv.org/pdf/2509.11575) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2509.11575)  
  *2025 · Forecasting, Anomaly Detection, Classification, QA-Reasoning, Causal Inferenc... · ToolUse, ReAct, RAG, MultiAgent, RL-Policy, Self-evolving*

- [Achieving Time Series Reasoning Requires Rethinking Model Design, Tasks Formulation, and Evaluation](https://arxiv.org/pdf/2502.01477) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2502.01477)  
  *2025 · QA & Forecasting & Classification*

- [Large Language models for Time Series Analysis: Techniques, Applications, and Challenges](https://arxiv.org/abs/2506.11040) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2506.11040)  
  *2025 · Forecasting, Classification, Anomaly Detection, Imputation*

- [Position: Empowering Time Series Reasoning with Multimodal LLMs](https://arxiv.org/pdf/2502.01477v1) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2502.01477)  
  *2025 · and Evaluation） · A-Perception,B-Reasoning · A: 四种时序表征策略——Raw Values直接文本化/Tokenization离散化编码/Encoding专用编码器压缩/Cross-Modality...*

- [Towards Interpretable and Trustworthy Time Series Reasoning: A BlueSky Vision](https://arxiv.org/pdf/2510.16980) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2510.16980)  
  *2025 · Forecasting & QA & Anomaly Detection & Classification*

### 2026

- [Agentic Trading: When LLM Agents Meet Financial Markets](https://arxiv.org/pdf/2605.19337) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2605.19337)  
  *2026 · Forecasting, Anomaly Detection, Classification · ToolUse, ReAct, RAG, MultiAgent, RL-Policy, Self-evolving · Finance-Trading*

- [Position: Beyond Model-Centric Prediction—Agentic Time Series Forecasting](https://arxiv.org/pdf/2602.01776) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2602.01776)  
  *2026 · Forecasting · ToolUse, ReAct, RAG, MultiAgent, RL-Policy, Self-evolving, AutoML, ProcMem*

### Year Unknown / To Be Checked

- [From Prompts to Agents: A Comprehensive Survey of LLM-Driven Time Series Analysis](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=6614598)  
  [![Paper](https://img.shields.io/badge/Paper-Link-blue.svg)](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=6614598)  
  *Forecasting, Anomaly Detection, Classification, Imputation, QA-Reasoning · ToolUse, RAG, MultiAgent, Self-evolving/Reflection*


## Benchmarks and Datasets

### 2020

- [ForecastQA: A Question Answering Challenge for Event Forecasting with Temporal Text Data](https://arxiv.org/pdf/2005.00792) (2020)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2005.00792)  
  *2020 · QA*

### 2021

- [(VISUELLE) Well Googled is Half Done: Multimodal Forecasting of New Fashion Product Sales with Image-based Google Trends](https://arxiv.org/pdf/2109.09824) (2021)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2109.09824)  
  *2021 · Forecasting · Retail*

### 2023

- [DOW 30](https://arxiv.org/pdf/2306.03763) (2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2306.03763)  
  *2023 · Classification · Finance-Trading*

### 2024

- [(CiK) Context is Key: A Benchmark for Forecasting with Essential Textual Information](https://arxiv.org/pdf/2410.18959) (2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2410.18959)  
  *2024 · Forecasting*

- [(NewsForecast) From News to Forecast: Integrating Event Analysis in LLM-Based Time Series Forecasting with Reflection](https://arxiv.org/pdf/2409.17515) (2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2409.17515)  
  *2024 · Forecasting*

- [(TTC) Multi-Modal Forecaster: Jointly Predicting Time Series and Textual Data](https://arxiv.org/pdf/2411.06735) (2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2411.06735)  
  *2024 · Forecasting*

- [Can LLMs Understand Time Series Anomalies?](https://arxiv.org/pdf/2410.05440) (2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2410.05440)  
  *2024 · Anomaly Detection*

- [Evaluating Large Language Models on Time Series Feature Understanding: A Comprehensive Taxonomy and Benchmark](https://arxiv.org/pdf/2404.16563) (2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2404.16563)  
  *2024 · Classification & QA*

- [FNSPID: A Comprehensive Financial News Dataset in Time Series](https://arxiv.org/pdf/2402.06698) (2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2402.06698)  
  *2024 · Forecasting · Finance-Trading*

- [Gift-Eval](https://arxiv.org/pdf/2410.10393) (2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2410.10393)  
  *2024 · Forecasting*

- [Language Models Still Struggle to Zero-shot Reason about Time Series](https://arxiv.org/pdf/2404.11757) (2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2404.11757)  
  *2024 · QA-Reasoning, Forecasting*

- [Language Models Still Struggle to Zero-shot Reason about Time Series](https://arxiv.org/pdf/2404.11757) (2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2404.11757)  
  *2024 · QA & Forecasting*

- [LEMMA-RCA: A Large Multi-modal Multi-domain Dataset for Root Cause Analysis](https://arxiv.org/pdf/2406.05375) (2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2406.05375)  
  *2024 · Forecasting · IT & IoT*

- [Time-MMD: Multi-Domain Multimodal Dataset for Time Series Analysis](https://arxiv.org/pdf/2406.08627) (2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2406.08627)  
  *2024 · Forecasting*

- [TimeSeriesExam: A time series understanding exam](https://arxiv.org/pdf/2410.14752) (2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2410.14752)  
  *2024 · QA & Anomaly Detection & Classification*

### 2025

- [(EngineMT-QA) ITFormer: Bridging Time Series and Natural Language for Multi-Modal QA with Large-Scale Multitask Dataset](https://arxiv.org/pdf/2506.20093) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2506.20093)  
  *2025 · QA · Aero*

- [CaTS-Bench: Can Language Models Describe Time Series?](https://arxiv.org/pdf/2509.20823) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2509.20823)  
  *2025 · QA*

- [fev bench](https://arxiv.org/pdf/2509.26468) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2509.26468)  
  *2025 · Forecasting*

- [Fidel-TS: A High-Fidelity Multimodal Benchmark for Time Series Forecasting](https://arxiv.org/pdf/2509.24789) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2509.24789)  
  *2025 · Forecasting*

- [FinMultiTime: A Four-Modal Bilingual Dataset for Financial Time-Series Analysis](https://arxiv.org/pdf/2506.05019) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2506.05019)  
  *2025 · Forecasting · Finance-Trading*

- [Investigating Compositional Reasoning in Time Series Foundation Models](https://arxiv.org/pdf/2502.06037) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2502.06037)  
  *2025 · Forecasting*

- [MoTime: A Dataset Suite for Multimodal Time Series Forecasting](https://arxiv.org/pdf/2505.15072) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2505.15072)  
  *2025 · Forecasting*

- [MTBench](https://arxiv.org/pdf/2503.16858) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2503.16858)  
  *2025 · Forecasting, Classification, QA*

- [Time-MQA](https://arxiv.org/pdf/2503.01875) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2503.01875)  
  *2025 · Forecasting, Imputation, Anomaly Detection, Classification, QA*

- [TIME-RA: Towards Time Series Reasoning for Anomaly Diagnosis with LLM Feedback](https://arxiv.org/pdf/2507.15066) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2507.15066)  
  *2025 · Anomaly Detection, Classification, QA-Reasoning*

- [TimeIMM](https://arxiv.org/pdf/2506.10412) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2506.10412)  
  *2025 · Forecasting*

- [TimeSeriesGym: A Scalable Benchmark for (Time Series) Machine Learning Engineering Agents](https://arxiv.org/pdf/2505.13291) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2505.13291)  
  *2025 · Forecasting, Classification, Anomaly Detection, QA-Reasoning, Regression, Imp...*

- [When LLM Meets Time Series: Can LLMs Perform Multistep Time Series Reasoning and Inference](https://arxiv.org/pdf/2509.01822) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2509.01822)  
  *2025 · Forecasting, Anomaly Detection, QA-Reasoning, Classification · General/Energy/Climate/Finance/Healthcare*

### 2026

- [ARFBench](https://arxiv.org/pdf/2604.21199) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2604.21199)  
  *2026 · QA-Reasoning, Anomaly Detection · Observability/Software*

- [Dr-CiK: A Testbed for Foresight-Driven Agents](https://arxiv.org/pdf/2605.27904) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2605.27904)  
  *2026 · Forecasting*

- [FinTexTS: Financial Text-Paired Time-Series Dataset via Semantic-Based and Multi-Level Pairing](https://arxiv.org/pdf/2603.02702) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2603.02702)  
  *2026 · Forecasting*

- [Foresight Arena: An On-Chain Benchmark for Evaluating AI Forecasting Agents](https://arxiv.org/pdf/2605.00420) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2605.00420)  
  *2026 · Forecasting · ToolUse, Benchmark, On-chain Verification · General/Prediction Markets*

- [HEARTS: Benchmarking LLM Reasoning on Health Time Series](https://arxiv.org/pdf/2603.06638) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2603.06638)  
  *2026 · Classification & Forecasting & Imputation & QA · Health*

- [It's TIME: Towards the Next Generation of Time Series Forecasting Benchmarks](https://arxiv.org/pdf/2602.12147) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2602.12147)  
  *2026 · Forecasting*

- [MMTS-Bench](https://arxiv.org/pdf/2602.08588) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2602.08588)  
  *2026 · QA-Reasoning, Classification*

- [TemporalBench: A Benchmark for Evaluating LLM-Based Agents on Contextual and Event-Informed Time Series Tasks](https://arxiv.org/pdf/2602.13272) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2602.13272)  
  *2026 · Forecasting, QA, Anomaly Detection*

- [TFRBench: A Reasoning Benchmark for Evaluating Forecasting Systems](https://arxiv.org/pdf/2604.05364) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2604.05364)  
  *2026 · Forecasting*

- [TimeSeriesExamAgent](https://arxiv.org/pdf/2604.10291) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2604.10291)  
  *2026 · QA, Anomaly Detection*

- [TSAQA](https://arxiv.org/pdf/2601.23204v1) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2601.23204)  
  *2026 · Anomaly Detection, Classification, QA-Reasoning*

- [TSRBench: A Comprehensive Multi-task Multi-modal Time Series Reasoning Benchmark for Generalist Models](https://arxiv.org/pdf/2601.18744) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2601.18744)  
  *2026 · Forecasting, Anomaly Detection, QA-Reasoning, Classification*

### Year Unknown / To Be Checked

- [Hybrid Deep Sequential Modeling for Social Text-Driven Stock Prediction](https://dl.acm.org/doi/10.1145/3269206.3269290)  
  [![ACM](https://img.shields.io/badge/ACM-DL-0073e6.svg)](https://dl.acm.org/doi/10.1145/3269206.3269290)  
  *Classification · Finance-Trading*

- [LLM Agents Struggle at Engineering Time Series Solutions](https://openreview.net/pdf?id=04fwpztRMB)  
  [![OpenReview](https://img.shields.io/badge/OpenReview-8c1b13.svg)](https://openreview.net/pdf?id=04fwpztRMB)  
  *Forecasting, Anomaly Detection, Classification, Imputation, Time Series Under... · AutoML, ToolUse, ReAct (注：评测对象如 AIDE, OpenHands 均依赖于 ToolUse/CodeAct 交互模式，且任务...*

- [Stock Movement Prediction from Tweets and Historical Prices](https://aclanthology.org/P18-1183.pdf)  
  [![Paper](https://img.shields.io/badge/Paper-Link-blue.svg)](https://aclanthology.org/P18-1183.pdf)  
  *Classification · Finance-Trading*


## Time Series Foundation Models

### 2023

- [Lag-Llama: Towards Foundation Models for Probabilistic Time Series Forecasting](https://arxiv.org/pdf/2310.08278) (2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2310.08278)  
  *2023 · Forecasting*

- [TimeGPT-1](https://arxiv.org/pdf/2310.03589) (2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2310.03589)  
  *2023 · Forecasting*

- [TimesFM 2.5](https://arxiv.org/pdf/2310.10688) (2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2310.10688)  
  *2023 · Forecasting*

### 2024

- [Chronos](https://arxiv.org/pdf/2403.07815) (2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2403.07815)  
  *2024 · Forecasting*

- [Moirai](https://arxiv.org/pdf/2402.02592) (2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2402.02592)  
  *2024 · Forecasting*

- [MOMENT: A Family of Open Time-series Foundation Models](https://arxiv.org/pdf/2402.03885) (2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2402.03885)  
  *2024 · Forecasting, Classification, Anomaly Detection, Imputation*

- [TimeMoE](https://arxiv.org/pdf/2409.16040) (2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2409.16040)  
  *2024 · Forecasting*

- [Timer](https://arxiv.org/pdf/2402.02368) (2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2402.02368)  
  *2024 · Forecasting, Imputation*

- [Tiny Time Mixers (TTMs): Fast Pre-trained Models for Enhanced Zero/Few-Shot Forecasting of Multivariate Time Series](https://arxiv.org/pdf/2401.03955) (2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2401.03955)  
  *2024 · Forecasting*

- [Toto](https://arxiv.org/pdf/2407.07874) (2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2407.07874)  
  *2024 · Forecasting*

- [UniTS: Building a Unified Time Series Model](https://arxiv.org/pdf/2403.00131) (2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2403.00131)  
  *2024 · Forecasting, Classification, Anomaly Detection, Imputation*

### 2025

- [Chronos-2](https://arxiv.org/pdf/2510.15821v1) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2510.15821)  
  *2025 · Forecasting*

- [GTM: A General Time-series Model for Enhanced Representation Learning of Time-Series Data](https://arxiv.org/pdf/2502.03264) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2502.03264)  
  *2025 · Forecasting, Classification, Anomaly Detection, Imputation*

- [LightGTS: A Lightweight General Time Series Forecasting Model](https://arxiv.org/pdf/2506.06005) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2506.06005)  
  *2025 · Forecasting*

- [Moirai 2.0: When Less Is More for Time Series Forecasting](https://arxiv.org/pdf/2511.11698) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2511.11698)  
  *2025 · Forecasting*

- [Multi-Modal View Enhanced Large Vision Models for Long-Term Time Series Forecasting](https://arxiv.org/pdf/2505.24003) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2505.24003)  
  *2025 · Forecasting · A: 多模态视图感知——数值视图直接编码原始序列，视觉视图通过period-based imaging将时序转为2D图像由MAE编码；backcast-r...*

- [Revitalizing Canonical Pre-Alignment for Irregular Multivariate Time Series Forecasting](https://arxiv.org/pdf/2508.01971) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2508.01971)  
  *2025 · Forecasting · A: CPA预处理将所有变量对齐到统一时间轴以缓解变量间异步性(Sec 3.2); Pre-Convolution模块通过1x3和1x1卷积平滑零填充序列...*

- [Sundial](https://arxiv.org/pdf/2502.00816) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2502.00816)  
  *2025 · Forecasting*

- [Synthetic Series-Symbol Data Generation for Time Series Foundation Models](https://arxiv.org/pdf/2510.08445) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2510.08445)  
  *2025 · Forecasting*

- [TabPFN-TS](https://arxiv.org/pdf/2501.02945) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2501.02945)  
  *2025 · Forecasting*

- [TiREX](https://arxiv.org/pdf/2505.23719) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2505.23719)  
  *2025 · Forecasting*

- [TS-RAG: Retrieval-Augmented Generation based Time Series Foundation Models are Stronger Zero-Shot Forecaster](https://arxiv.org/pdf/2503.07649) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2503.07649)  
  *2025 · Forecasting · A: 使用TSFM编码器(Chronos-Bolt)对输入时序进行编码生成嵌入表示(Sec 3.2); 检索编码器对查询时序和知识库中的时序上下文生成嵌入...*

- [TSPulse: Tiny Pre-Trained Models with Disentangled Representations for Rapid Time-Series Analysis](https://arxiv.org/pdf/2505.13033) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2505.13033)  
  *2025 · Classification, Anomaly Detection, Imputation, Similarity Search*

### 2026

- [AME-TS: Anchored Mixture-of-Experts for Time Series Forecasting](https://arxiv.org/pdf/2605.25166) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2605.25166)  
  *2026 · Forecasting*

- [MEMTS: Internalizing Domain Knowledge via Parameterized Memory for Retrieval-Free Domain Adaptation of Time Series Foundation Models](https://arxiv.org/pdf/2602.13783) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2602.13783)  
  *2026 · Forecasting · D: Knowledge Persistence Module(KPM)将领域特定时序模式(周期性/趋势等)内化为参数化隐原型，Context Encod... · ProcMem*

- [Time Series Causal Discovery via Context-Conditioned and Causality-Augmented Pretraining](https://arxiv.org/pdf/2605.26759) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2605.26759)  
  *2026 · Causal Discovery & Anomaly Detection · WorldModel*

- [Timer-S1](https://arxiv.org/pdf/2603.04791) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2603.04791)  
  *2026 · Forecasting*

- [Toto 2.0](https://arxiv.org/pdf/2605.20119v1) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2605.20119)  
  *2026 · Forecasting*

- [TS-Memory: Plug-and-Play Memory for Time Series Foundation Models](https://arxiv.org/pdf/2602.11550) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2602.11550)  
  *2026 · Forecasting*

### Year Unknown / To Be Checked

- Falcon-X

- [TimeCAP: A channel aware pre training framework for multivariate time series forecasting](https://ore.exeter.ac.uk/ndownloader/files/60062780)  
  [![Paper](https://img.shields.io/badge/Paper-Link-blue.svg)](https://ore.exeter.ac.uk/ndownloader/files/60062780)  
  *Forecasting*


## LLM4TS: Translation and Alignment

### 2022

- [PromptCast: A New Prompt-based Learning Paradigm for Time Series Forecasting](https://arxiv.org/pdf/2210.08964) (2022)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2210.08964)  
  *2022 · Forecasting*

### 2023

- [LLM4TS: Two-Stage Fine-Tuning for Time-Series Forecasting with Pre-trained LLMs](https://arxiv.org/pdf/2308.08469) (2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2308.08469)  
  *2023 · Forecasting*

- [One Fits All: Power General Time Series Analysis by Pretrained LM](https://arxiv.org/pdf/2302.11939) (2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2302.11939)  
  *2023 · Anomaly Detection,Classification,Forecasting,Imputation*

- [TEMPO: Prompt-based Generative Pre-trained Transformer for Time Series Forecasting](https://arxiv.org/pdf/2310.04948) (2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2310.04948)  
  *2023 · Forecasting*

- [TEST: Text Prototype Aligned Embedding to Activate LLM's Ability for Time Series](https://arxiv.org/pdf/2308.08241) (2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2308.08241)  
  *2023 · Forecasting, Classification, Anomaly Detection*

- [Time-LLM](https://arxiv.org/pdf/2310.01728) (2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2310.01728)  
  *2023 · Forecasting*

### 2024

- [$S^2$IP-LLM: Semantic Space Informed Prompt Learning with LLM for Time Series Forecasting](https://arxiv.org/pdf/2403.05798) (2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2403.05798)  
  *2024 · Forecasting*

- [A Picture is Worth A Thousand Numbers: Enabling LLMs Reason about Time Series via Visualization](https://arxiv.org/pdf/2411.06018) (2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2411.06018)  
  *2024 · Classification · A: 可视化建模——将数值时序数据转化为时域/频域图像表示保留时间戳/语义标签/跨维度特征(Sec 3 VL-Time Planning Stage); ...*

- [AutoTimes: Autoregressive Time Series Forecasters via Large Language Models](https://arxiv.org/pdf/2402.02370) (2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2402.02370)  
  *2024 · Forecasting*

- [CALF](https://arxiv.org/pdf/2403.07300) (2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2403.07300)  
  *2024 · Forecasting*

- [ChatTime: A Unified Multimodal Time Series Foundation Model Bridging Numerical and Textual Data](https://arxiv.org/pdf/2412.11376) (2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2412.11376)  
  *2024 · Forecasting, QA*

- [ChatTS: Aligning Time Series with LLMs via Synthetic Data for Enhanced Understanding and Reasoning](https://arxiv.org/pdf/2412.03104) (2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2412.03104)  
  *2024 · Forecasting, QA, Classification*

- [Multi-Patch Prediction: Adapting LLMs for Time Series Representation Learning](https://arxiv.org/pdf/2402.04852) (2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2402.04852)  
  *2024 · Forecasting, Classification*

- [MultiCast: Zero-Shot Multivariate Time Series Forecasting Using LLMs](https://arxiv.org/pdf/2405.14748) (2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2405.14748)  
  *2024 · Forecasting · A: 三种维度复用技术将多变量时序映射为LLM兼容的一维token序列——digit-interleaving按位交错/value-interleavin...*

- [TimeCMA](https://arxiv.org/pdf/2406.01638) (2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2406.01638)  
  *2024 · Forecasting*

- [Towards Time Series Reasoning with LLMs](https://arxiv.org/pdf/2409.11376) (2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2409.11376)  
  *2024 · QA & Classification · A: 训练轻量级multi-head self-attention编码器将patchified时序投影到LLM词嵌入空间(Sec 3.1); B: 通过C...*

### 2025

- [AXIS: Explainable Time Series Anomaly Detection with Large Language Models](https://arxiv.org/pdf/2509.24378) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2509.24378)  
  *2025 · Anomaly Detection*

- [DP-GPT4MTS: Dual-Prompt Large Language Model for Textual-Numerical Time Series Forecasting](https://arxiv.org/pdf/2508.04239) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2508.04239)  
  *2025 · Forecasting*

- [FreqLLM](https://www.ijcai.org/proceedings/2025/377) (2025)  
  [![Paper](https://img.shields.io/badge/Paper-Link-blue.svg)](https://www.ijcai.org/proceedings/2025/377)  
  *2025 · Forecasting*

- [From Values to Tokens: An LLM-Driven Framework for Context-aware Time Series Forecasting via Symbolic Discretization](https://arxiv.org/pdf/2508.09191v1) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2508.09191)  
  *2025 · Forecasting*

- [FSCA](https://arxiv.org/pdf/2501.03747) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2501.03747)  
  *2025 · Forecasting,Classification*

- [GEM: Empowering MLLM for Grounded ECG Understanding with Time Series and Images](https://arxiv.org/pdf/2503.06073) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2503.06073)  
  *2025 · Classification & QA · A: 双编码器架构——ECG时间序列编码器(ECG-CoCa预训练)与ECG图像编码器(CLIP from LLaVA)分别提取特征(Sec 3.2); ...*

- [Human in the Loop Adaptive Optimization for Improved Time Series Forecasting](https://arxiv.org/pdf/2505.15354) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2505.15354)  
  *2025 · Forecasting*

- [Language in the Flow of Time: Time-Series-Paired Texts Weaved into a Unified Temporal Narrative](https://arxiv.org/pdf/2502.08942) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2502.08942)  
  *2025 · Forecasting & Imputation · A: 利用预训练LLM(GPT-2/BERT/LLaMA2)将时间戳配对文本编码为嵌入向量，再通过MLP投影到低维空间作为辅助变量拼接至原始时间序列，实现...*

- [Let LLMs Speak Embedding Languages: Generative Text Embeddings via Iterative Contrastive Refinement](https://arxiv.org/pdf/2509.24291) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2509.24291)  
  *2025 · Forecasting*

- [OpenTSLM: Time-Series Language Models for Reasoning over Multivariate Medical Text- and Time-Series Data](https://arxiv.org/pdf/2510.02410) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2510.02410)  
  *2025 · QA · A: PatchTST/Chronos-2编码器提取时序patch特征并加入位置编码(Sec 3.1); OpenTSLM-SP通过MLP投影将时序tok...*

- [SE-LLM](https://arxiv.org/pdf/2508.07697) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2508.07697)  
  *2025 · Forecasting*

- [Semantic-Enhanced Time-Series Forecasting via Large Language Models](https://arxiv.org/pdf/2508.07697) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2508.07697)  
  *2025 · Forecasting · A: 滑动窗口分段+Time Encoder投影为TS Embedding，从LLM词嵌入矩阵线性投影构建语义原型S，交叉注意力将时序嵌入与语义空间对齐产...*

- [Teaching Time Series to See and Speak: Forecasting with Aligned Visual and Textual Perspectives](https://arxiv.org/pdf/2506.24124) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2506.24124)  
  *2025 · Forecasting*

- [Time-Llama](https://arxiv.org/pdf/2502.13725) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2502.13725)  
  *2025 · Forecasting*

- [TimeXL: Explainable Multi-modal Time Series Prediction with LLM-in-the-Loop](https://arxiv.org/pdf/2503.01013) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2503.01013)  
  *2025 · Forecasting*

- [TS-Reasoner: Aligning Time Series Foundation Models with LLM Reasoning](https://arxiv.org/pdf/2510.03519) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2510.03519)  
  *2025 · QA & Classification · A: 使用冻结的预训练TSFM(TimesFM)编码patched时序为紧凑嵌入，再通过MLP适配器投影到LLM输入嵌入空间(Sec 3.1); B: 通...*

- [UniCast: A Unified Multimodal Prompting Framework for Time Series Forecasting](https://arxiv.org/pdf/2508.11954) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2508.11954)  
  *2025 · Forecasting · A: 冻结的CLIP/BLIP视觉编码器和Qwen/LLaMA文本编码器提取模态嵌入，Transformer-based Context Distille...*

### 2026

- [Bridging Temporal and Textual Modalities: A Multimodal Framework for Automated Cloud Failure Root Cause Analysis](https://arxiv.org/pdf/2601.04709) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2601.04709)  
  *2026 · QA · A: Patch分割+单token语义压缩将时序片段映射为语义token(Sec 3.1); Time Series Encoder通过门控交叉注意力将时...*

- [Factorize to Generalize: Retrieval-Guided Invariant-Dynamic Decomposition for Time Series Forecasting](https://arxiv.org/pdf/2605.24911) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2605.24911)  
  *2026 · Forecasting · Sec 2) / B-Reasoning: 检索引导路由机制将表示分解为不变/动态分量(不变分支保留稳定共享结构，动态分支捕获查询特定变异)，正交解耦正则...*

- [LLM-based TSC](https://arxiv.org/pdf/2601.09971) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2601.09971)  
  *2026 · Classification*

- [Multi-scale hypergraph meets LLMs: Aligning large language models for time series analysis](https://arxiv.org/pdf/2602.04369) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2602.04369)  
  *2026 · Forecasting & Classification · A: 多尺度提取模块(ME)将原始时序分层聚合为多尺度时序特征，超边机制用可学习超边捕获组内隐式交互并减少噪声，跨模态对齐(CMA)模块通过多头交叉注意力...*

- [PaP-NF: Probabilistic Long-Term Time Series Forecasting via Prefix-as-Prompt Reprogramming and Normalizing Flows](https://arxiv.org/pdf/2605.23219) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2605.23219)  
  *2026 · Forecasting · c)条件归一化流生成预测分布(Sec 3.4)*

- [STaT: Resolving Shape Distortion in Non-Stationary Time Series via Tri-Modal Synergy](https://arxiv.org/pdf/2605.25943) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2605.25943)  
  *2026 · Forecasting*

- [What if Tomorrow is the World Cup Final? Counterfactual Time Series Forecasting with Textual Conditions](https://arxiv.org/pdf/2605.14422) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2605.14422)  
  *2026 · Forecasting*

### Year Unknown / To Be Checked

- [JoLT: Jointly Learned Representations of Language and Time-Series](https://openreview.net/pdf?id=UVF1AMBj9u)  
  [![OpenReview](https://img.shields.io/badge/OpenReview-8c1b13.svg)](https://openreview.net/pdf?id=UVF1AMBj9u)  
  *Classification · A: 采用patch-based时序编码器提取时序特征，利用预训练LLM文本编码器提取文本语义，通过对比学习将两种模态对齐到共享嵌入空间，实现时序-文本跨...*

- [STEM-LTS: Integrating Semantic-Temporal Dynamics in LLM-driven Time Series Analysis](https://ojs.aaai.org/index.php/AAAI/article/view/34447)  
  [![Paper](https://img.shields.io/badge/Paper-Link-blue.svg)](https://ojs.aaai.org/index.php/AAAI/article/view/34447)  
  *Forecasting*


## LLM4TS: Temporal Reasoning

### 2024

- [Can LLMs Serve as Time Series Anomaly Detectors?](https://arxiv.org/pdf/2408.03475) (2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2408.03475)  
  *2024 · Anomaly Detection*

- [LSTPrompt: Large Language Models as Zero-Shot Time Series Forecasters by Long-Short-Term Prompting](https://arxiv.org/pdf/2402.16132) (2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2402.16132)  
  *2024 · Forecasting · A: 采用LLMTime风格的数值字符串输入方式将时序数据以逗号分隔数字形式直接输入LLM(Sec 3.1); B: TimeDecomp将TSF分解为短...*

### 2025

- [Augur: Modeling Covariate Causal Associations in Time Series via Large Language Models](https://arxiv.org/pdf/2510.07858) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2510.07858)  
  *2025 · Forecasting*

- [Can Slow-Thinking LLMs Reason Over Time? Empirical Studies in Time Series Forecasting](https://arxiv.org/pdf/2505.24511) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2505.24511)  
  *2025 · Forecasting*

- [Chain-of-thought Reviewing and Correction for Time Series Question Answering](https://arxiv.org/pdf/2512.22627) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2512.22627)  
  *2025 · QA · A: 时序数据文本化后输入LLM保留原始数值尺度信息(Sec 2); B: Worker LLM生成结构化逐步CoT推理链(Sec 2.1); Revie...*

- [Eliciting Chain-of-Thought Reasoning for Time Series Analysis using Reinforcement Learning](https://arxiv.org/pdf/2510.01116) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2510.01116)  
  *2025 · Forecasting, Classification, QA-Reasoning · RL-Policy*

- [Learning to Reason Over Time: Timeline Self-Reflection for Improved Temporal Reasoning in Language Models](https://arxiv.org/pdf/2504.05258) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2504.05258)  
  *2025 · QA · A: 将时序上下文中的时间事件提取并组织为有序时间线(Sec 2.1 Stage II); B: 多阶段时序推理——初始CoT推理链(Stage I)/时...*

- [Retrieval-augmented Large Language Models for Financial Time Series Forecasting](https://arxiv.org/pdf/2502.05878) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2502.05878)  
  *2025 · Forecasting · A: FinSeer从候选池中检索与query相关的历史时序片段，候选池包含34种金融指标(Sec 3.1); B: StockLLM基于检索到的历史模式...*

- [T3LLM](https://arxiv.org/pdf/2512.22627) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2512.22627)  
  *2025 · QA-Reasoning, Classification, Anomaly Detection, Forecasting, Imputation · Multi-LLM协作推理修正*

- [Time Series Forecasting as Reasoning: A Slow-Thinking Approach with Reinforced LLMs](https://arxiv.org/pdf/2506.10630) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2506.10630)  
  *2025 · Forecasting · RL-Policy*

- [Time-R1: Towards Comprehensive Temporal Reasoning in LLMs](https://arxiv.org/pdf/2505.13508) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2505.13508)  
  *2025 · QA & Forecasting · A: 以新闻标题和摘要文本作为输入通过LLM tokenizer进行Symbolic感知将事件描述映射为token序列(Sec 3.2 Stage1); ...*

- [TimeMaster: Training Time-Series Multimodal LLMs to Reason via Reinforcement Learning](https://arxiv.org/pdf/2506.13705) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2506.13705)  
  *2025 · Classification & QA · A: 将时序可视化为图像输入MLLM，利用视觉编码器感知时序模式(Sec 3.1); B: 通过think标签生成CoT推理链包含模式识别/趋势分析/因果...*

- [TimeOmni-1: Incentivizing Complex Reasoning with Time Series in Large Language Models](https://arxiv.org/pdf/2509.24803) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2509.24803)  
  *2025 · Forecasting, Classification, QA-Reasoning · RL-Policy*

- [Trading-R1: Financial Trading with LLM Reasoning via Reinforcement Learning](https://arxiv.org/pdf/2509.11420) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2509.11420)  
  *2025 · Forecasting & Classification · A: 多模态感知——整合技术市场数据(价格/EMA/波动率)/基本面数据/新闻/内部人情绪/宏观经济指标等多源异构金融信息(Sec 3.2); B: 结构...*

- [Training-Free Time Series Classification via In-Context Reasoning with LLM Agents (FETA)](https://arxiv.org/pdf/2510.05950) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2510.05950)  
  *2025 · Classification · MultiAgent(Pipeline), RAG*

### 2026

- [Adaptive Time Series Reasoning via Segment Selection](https://arxiv.org/pdf/2602.18645) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2602.18645)  
  *2026 · QA-Reasoning · RL-Policy, ToolUse*

- [PATRA](https://arxiv.org/pdf/2602.23161) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2602.23161)  
  *2026 · QA-Reasoning · 2]防止异构任务间的reward hacking，激励连贯CoT生成（Sec 3.2）*

- [Rationale-Grounded In-Context Learning for Time Series Reasoning with Multimodal Large Language Models](https://arxiv.org/pdf/2601.02968) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2601.02968)  
  *2026 · Classification · A: MLLM接收时序可视化图表作为视觉输入(Sec 3.2); TabPFN编码器提取时序数据嵌入用于数据驱动检索(Sec 3.2); 文本嵌入模型编码...*

- [Reasoning through Verifiable Forecast Actions: Consistency-Grounded RL for Financial LLMs](https://arxiv.org/pdf/2605.21975) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2605.21975)  
  *2026 · Forecasting/QA · ToolUse/RL-Policy*

- [Reasoning-Aware Training for Time Series Forecasting](https://arxiv.org/pdf/2605.08625v1) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2605.08625)  
  *2026 · Forecasting*

- [Time Series Reasoning via Process-Verifiable Thinking Data Synthesis and Scheduling for Tailored LLM Reasoning](https://arxiv.org/pdf/2602.07830) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2602.07830)  
  *2026 · QA-Reasoning, Anomaly Detection, Classification · RL-Policy*

- [TimeOmni-VL: Unified Models for Time Series Understanding and Generation](https://arxiv.org/pdf/2602.17149) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2602.17149)  
  *2026 · Forecasting & Imputation · A: Bi-TSI将时序转换为高保真TS-image表示，含RFN稳定动态范围投影/Encoding Capacity Control防止隐式下采样/89...*

### Year Unknown / To Be Checked

- [Delving into Large Language Models for Effective Time-Series Anomaly Detection](https://openreview.net/pdf?id=6rpy7X1Of8)  
  [![OpenReview](https://img.shields.io/badge/OpenReview-8c1b13.svg)](https://openreview.net/pdf?id=6rpy7X1Of8)  
  *Anomaly Detection · A: 系统比较多种时序表示方法(原始数值序列/tokenization离散化/patch编码等)将时序信号输入LLM的方式研究不同表示对异常检测效果的影响...*


## Agentic Time Series Systems

Papers in this section are placed according to their **primary contribution**. Many systems span multiple layers; tags such as ToolUse, RAG, MultiAgent, RL-Policy, AutoML, WorldModel, and ProcMem indicate secondary mechanisms.

### Perception Agents

#### 2024

- [CityGPT: Towards Urban IoT Learning, Analysis and Interaction with Multi-Agent System](https://arxiv.org/pdf/2405.14691) (2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2405.14691)  
  *2024 · Forecasting, Spatial Analysis · MultiAgent, AutoML, ToolUse · IoT/Smart City*

- [Decoding Time Series with LLMs: A Multi-Agent Framework for Cross-Domain Annotation](https://arxiv.org/pdf/2410.17462) (2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2410.17462)  
  *2024 · Classification · MultiAgent*

#### 2025

- [Hierarchical AI-Meteorologist: LLM-Agent System for Multi-Scale and Explainable Weather Forecast Reporting](https://arxiv.org/pdf/2511.23387) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2511.23387)  
  *2025 · Forecasting · MultiAgent · Weather/Climate*

- [TimeCAP: Learning to Contextualize, Augment, and Predict Time Series Events with Large Language Model Agents](https://arxiv.org/pdf/2502.11418) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2502.11418)  
  *2025 · Classification · MultiAgent, RAG*

#### 2026

- [AGCD: Agent-Guided Cross-Modal Decoding for Weather Forecasting](https://arxiv.org/pdf/2603.15260) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2603.15260)  
  *2026 · Forecasting · MultiAgent · Weather/Climate*

- [Grammar of the Wave: Towards Explainable Multivariate Time Series Event Detection via Neuro-Symbolic VLM Agents](https://arxiv.org/pdf/2603.11479) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2603.11479)  
  *2026 · Event Detection · MultiAgent, ToolUse · Energy (Oil & Gas)*

- [MarsTSC: Empowering VLMs for Few-Shot Multimodal Time Series Classification via Tailored Agentic Reasoning](https://arxiv.org/pdf/2605.09395) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2605.09395)  
  *2026 · Classification · MultiAgent, Self-evolving, ProcMem*

- [MAS4TS: Visual Reasoning over Time Series via Multi-Agent System](https://arxiv.org/pdf/2602.03026) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2602.03026)  
  *2026 · Forecasting,Anomaly Detection,Classification,Imputation · MultiAgent, ToolUse*

- [Optimizing Multi-Agent Weather Captioning via Text Gradient Descent: A Training-Free Approach with Consensus-Aware Gradient Fusion](https://arxiv.org/pdf/2603.21673) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2603.21673)  
  *2026 · Classification,QA-Reasoning · MultiAgent, Self-evolving · Weather/Climate*

- [TS-Debate: Multimodal Collaborative Debate for Zero-Shot Time Series Reasoning](https://arxiv.org/pdf/2601.19151) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2601.19151)  
  *2026 · Classification, Forecasting, QA-Reasoning, Anomaly Detection, Imputation · MultiAgent, ToolUse*

#### Year Unknown / To Be Checked

- [ChatKG: Visualizing Time-Series Patterns Aided by Intelligent Agents and a Knowledge Graph](https://www.sciencedirect.com/science/article/pii/S0097849324002279)  
  [![Paper](https://img.shields.io/badge/Paper-Link-blue.svg)](https://www.sciencedirect.com/science/article/pii/S0097849324002279)  
  *Time Series Understanding, Pattern Discovery, QA-Reasoning, Exploratory Analysis · MultiAgent, ToolUse, RAG, KnowledgeGraph-Memory · Visual Analytics / Historical Time Series Analysis / Life Expectancy Analysis*


### Reasoning Agents

#### 2024

- [TS-Reasoner: Domain-Oriented Time Series Inference Agents for Reasoning and Automated Analysis](https://arxiv.org/pdf/2410.04047) (2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2410.04047)  
  *2024 · Forecasting, Anomaly Detection, QA-Reasoning, Classification · ToolUse, ReAct*

#### 2025

- [Argos: Agentic Time-Series Anomaly Detection with Autonomous Rule Generation via LLMs](https://arxiv.org/pdf/2501.14170) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2501.14170)  
  *2025 · Anomaly Detection · MultiAgent, AutoML · Cloud Infrastructure Monitoring (AIOps)*

- [Can Competition Enhance the Proficiency of Agents Powered by Large Language Models in the Realm of News-driven Time Series Forecasting?](https://arxiv.org/pdf/2504.10210) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2504.10210)  
  *2025 · Forecasting · MultiAgent, Self-evolving · News-driven / General*

- [Can Multimodal LLMs Perform Time Series Anomaly Detection?](https://arxiv.org/pdf/2502.17812) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2502.17812)  
  *2025 · Anomaly Detection · MultiAgent, ToolUse*

- [MONAQ: Multi-Objective Neural Architecture Querying for Time-Series Analysis on Resource-Constrained Devices](https://arxiv.org/pdf/2505.10607) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2505.10607)  
  *2025 · Classification, Regression · MultiAgent, AutoML · Edge/IoT (HAR, Health Monitoring, Energy)*

- [TS-Agent: A Time Series Reasoning Agent with Iterative Statistical Insight Gathering (ReAct-style)](https://arxiv.org/pdf/2510.07432) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2510.07432)  
  *2025 · Anomaly Detection, Classification, QA-Reasoning · ReAct, ToolUse*

#### 2026

- [AnomaMind: Agentic Time Series Anomaly Detection with Tool-Augmented Reasoning](https://arxiv.org/pdf/2602.13807) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2602.13807)  
  *2026 · Anomaly Detection · ToolUse, ReAct, RL-Policy*

- [LLM-Enhanced Reinforcement Learning for Time Series Anomaly Detection](https://arxiv.org/pdf/2601.02511) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2601.02511)  
  *2026 · Anomaly Detection · RL-Policy*

- [SAGE: Detecting Time Series Anomalies Like an Expert: A Multi-Agent LLM Framework with Specialized Analyzers](https://arxiv.org/pdf/2605.05725) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2605.05725)  
  *2026 · Anomaly Detection · MultiAgent, ToolUse, RAG*

- [TimeART: Towards Agentic Time Series Reasoning via Tool-Augmentation](https://arxiv.org/pdf/2601.13653) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2601.13653)  
  *2026 · Forecasting,Anomaly Detection,QA-Reasoning · ToolUse, ReAct*

#### Year Unknown / To Be Checked

- [An Interpretable Agent-Assisted Pipeline for Statistical Anomaly Detection in IoT Temperature Time Series](https://www.mdpi.com/2079-9292/15/9/1840)  
  [![Paper](https://img.shields.io/badge/Paper-Link-blue.svg)](https://www.mdpi.com/2079-9292/15/9/1840)  
  *Anomaly Detection · Rule-based Agent-Assisted Selection · IoT / Edge Monitoring / Temperature Sensor Anomaly Detection*

- [MAS-LSTM: A Multi-Agent LSTM-Based Approach for Scalable Anomaly Detection in IIoT Networks](https://www.scilit.com/publications/mas-lstm)  
  [![Paper](https://img.shields.io/badge/Paper-Link-blue.svg)](https://www.scilit.com/publications/mas-lstm)  
  *Anomaly Detection · MultiAgent · Industrial IoT / Network Security / Intrusion & Anomaly Detection*


### Planning & Action Agents

#### 2025

- [DCATS: Empowering Time Series Forecasting with LLM-Agents](https://arxiv.org/pdf/2508.04231) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2508.04231)  
  *2025 · Forecasting · CoT · Traffic-Transport*

- [TimeCopilot](https://arxiv.org/pdf/2509.00616) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2509.00616)  
  *2025 · Forecasting · ToolUse, AutoML*

- [TimeSeriesScientist: A General-Purpose AI Agent for Time Series Analysis](https://arxiv.org/pdf/2510.01538) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2510.01538)  
  *2025 · Forecasting · MultiAgent, AutoML, ToolUse*

- [TS-Agent (金融) Structured Agentic Workflows for Financial Time-Series Modeling with LLMs and Reflective Feedback](https://arxiv.org/pdf/2508.13915) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2508.13915)  
  *2025 · Forecasting, Generation · S_v)记录每轮实验结果和代码配置，三类静态外部知识库——Case Bank(E_case)存储历史任务成功方法论用于case-based reasoni...*

#### 2026

- [Cast-R1: Learning Tool-Augmented Sequential Decision Policies for Time Series Forecasting](https://arxiv.org/pdf/2602.13802v1) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2602.13802)  
  *2026 · Forecasting · RL-Policy, ToolUse*

- [Nexus: An Agentic Framework for Time Series Forecasting](https://arxiv.org/pdf/2605.14389) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2605.14389)  
  *2026 · Forecasting · MultiAgent · Finance(Stock Market), Real Estate(Zillow)*

#### Year Unknown / To Be Checked

- [AutoLM](https://link.springer.com/content/pdf/10.1007/s12273-025-1385-7.pdf)  
  [![Springer](https://img.shields.io/badge/Springer-Link-6db33f.svg)](https://link.springer.com/content/pdf/10.1007/s12273-025-1385-7.pdf)  
  *Forecasting · MultiAgent, RAG, AutoML, ToolUse · Building Energy / Load Forecasting / Smart Building*

- [Many Minds, One Goal (MAFS): Time Series Forecasting via Sub-task Specialization and Inter-agent Cooperation](https://openreview.net/pdf?id=Uon41HfqR3)  
  [![OpenReview](https://img.shields.io/badge/OpenReview-8c1b13.svg)](https://openreview.net/pdf?id=Uon41HfqR3)  
  *Forecasting · MultiAgent*

- [MAT-AITSC: Multi-Agent Transformer-based Automated Imbalanced Time Series Classification with Hyperparameter Optimization](https://scholar.nycu.edu.tw/en/publications/multi-agent-transformer-based-automated-imbalanced-time-series-cl/)  
  [![Paper](https://img.shields.io/badge/Paper-Link-blue.svg)](https://scholar.nycu.edu.tw/en/publications/multi-agent-transformer-based-automated-imbalanced-time-series-cl/)  
  *Classification · MultiAgent, RL-Policy, AutoML*

- [MoiraiAgent: An Agentic Framework for Context-Aware Time-Series Forecasting](https://www.salesforce.com/blog/moiraiagent/)  
  [![Paper](https://img.shields.io/badge/Paper-Link-blue.svg)](https://www.salesforce.com/blog/moiraiagent/)  
  *Forecasting · ToolUse, LLM-Orchestration, AutoML*

- [Multi-Agent Adversarial Time Series Forecasting](https://openreview.net/forum?id=lj1qwU6Gxs)  
  [![OpenReview](https://img.shields.io/badge/OpenReview-8c1b13.svg)](https://openreview.net/forum?id=lj1qwU6Gxs)  
  *Forecasting · MultiAgent, RL-Policy · Finance-Trading, General*

- [TimeCIEL: Contextual Interactive Ensemble Learning for Time Series Classification](https://hal.science/hal-05053054v1/document)  
  [![Paper](https://img.shields.io/badge/Paper-Link-blue.svg)](https://hal.science/hal-05053054v1/document)  
  *Classification · MultiAgent*


### Memory & Knowledge Agents

#### 2023

- [FinMem: A Performance-Enhanced LLM Trading Agent with Layered Memory and Character Design](https://arxiv.org/pdf/2311.13743) (2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2311.13743)  
  *2023 · Trading · RAG, Self-evolving · Finance-Trading*

#### 2024

- [Agentic Retrieval-Augmented Generation for Time Series Analysis](https://arxiv.org/pdf/2408.14484) (2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2408.14484)  
  *2024 · Forecasting, Anomaly Detection, Classification, Imputation · MultiAgent, RAG, ReAct*

- [ColaCare: Enhancing Electronic Health Record Modeling through Large Language Model-Driven Multi-Agent Collaboration](https://arxiv.org/pdf/2410.02551) (2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2410.02551)  
  *2024 · Classification (Mortality & Readmission Prediction) · MultiAgent, RAG · Healthcare*

#### 2025

- [AD-AGENT: A Multi-agent Framework for End-to-end Anomaly Detection](https://arxiv.org/pdf/2505.12594) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2505.12594)  
  *2025 · Anomaly Detection · MultiAgent, ToolUse, RAG, AutoML*

- [AlphaCast: An Interaction-Driven Agentic Reasoning Framework for Cognition-Inspired Time Series Forecasting](https://arxiv.org/pdf/2511.08947v3) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2511.08947)  
  *2025 · Forecasting · ToolUse, RAG, Self-evolving · Energy/General*

- [CALM: Continuous, Adaptive, and LLM-Mediated Anomaly Detection in Time-Series Streams](https://arxiv.org/pdf/2508.21273) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2508.21273)  
  *2025 · Anomaly Detection · Self-evolving, AutoML*

- [Conversational Time Series Foundation Models: Towards Explainable and Effective Forecasting](https://arxiv.org/pdf/2512.16022) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2512.16022)  
  *2025 · Forecasting · A: LLM分析优化轨迹/交叉验证性能指标(MAE/MSE/SMAPE/CRPS)/数据集特征(趋势/季节性强度)执行Align-Match-Future... · ToolUse,RL-Policy*

- [ElliottAgents: A Natural Language-Driven Multi-Agent System for Stock Market Analysis and Prediction](https://arxiv.org/pdf/2507.03435v1) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2507.03435)  
  *2025 · Forecasting · MultiAgent, RAG, RL-Policy, ToolUse · Finance-Trading*

- [FLAIRR-TS: Forecasting LLM-Agents with Iterative Refinement and Retrieval for Time Series](https://arxiv.org/pdf/2508.19279) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2508.19279)  
  *2025 · Forecasting · MultiAgent, RAG, Self-evolving*

- [MERIT: Multi-Agent Collaboration for Unsupervised Time Series Representation Learning](https://aclanthology.org/2025.findings-acl.1231.pdf) (2025)  
  [![Paper](https://img.shields.io/badge/Paper-Link-blue.svg)](https://aclanthology.org/2025.findings-acl.1231.pdf)  
  *2025 · Classification, Forecasting, Anomaly Detection, Transfer Learning, Representa... · MultiAgent, RAG, ProcMem*

- [ZARA: Training-Free Motion Time-Series Reasoning via Evidence-Grounded LLM Agents](https://arxiv.org/pdf/2508.04038) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2508.04038)  
  *2025 · Classification · RAG, MultiAgent, CoT · General (Human Activity Recognition)*

#### 2026

- [CastFlow: Learning Role-Specialized Agentic Workflows for Time Series Forecasting](https://arxiv.org/pdf/2604.27840) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2604.27840)  
  *2026 · Forecasting · ToolUse, Self-evolving, ProcMem · Energy/General*

- [ChatAD: Reasoning-Enhanced Time-Series Anomaly Detection with Multi-Turn Instruction Evolution](https://arxiv.org/pdf/2601.13546) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2601.13546)  
  *2026 · Anomaly Detection,Classification,Imputation · MultiAgent, Self-evolving, ProcMem · General / Anomaly Detection*

- [MemCast: Memory-Driven Time Series Forecasting with Experience-Conditioned Reasoning](https://arxiv.org/pdf/2602.03164) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2602.03164)  
  *2026 · Forecasting · RAG, Self-evolving, ProcMem*

#### Year Unknown / To Be Checked

- [An Autonomous Large Language Model-Agent Framework for Transparent and Local Time Series Forecasting](https://advanced.onlinelibrary.wiley.com/doi/10.1002/aidi.202500236)  
  [![Paper](https://img.shields.io/badge/Paper-Link-blue.svg)](https://advanced.onlinelibrary.wiley.com/doi/10.1002/aidi.202500236)  
  *Forecasting, Anomaly Detection · ReAct, ToolUse, RAG, ProcMem*

- [SocioDojo: Building Lifelong Analytical Agents with Real-world Text and Time Series](https://openreview.net/pdf?id=s9z0HzWJJp)  
  [![OpenReview](https://img.shields.io/badge/OpenReview-8c1b13.svg)](https://openreview.net/pdf?id=s9z0HzWJJp)  
  *Forecasting · A: 多模态感知模块同时处理社会经济文本(新闻报道/报告)与时序数据(经济指标)从非结构化文本中提取事件与语义信息; B: 对社会经济趋势进行模式推理与因... · ToolUse,ProcMem*


### World-Model & Data Agents

#### 2023

- [A Multi-Agent Reinforcement Learning Framework for Optimizing Financial Trading Strategies based on TimesNet](https://dl.acm.org/doi/10.1016/j.eswa.2023.121502) (2023)  
  [![ACM](https://img.shields.io/badge/ACM-DL-0073e6.svg)](https://dl.acm.org/doi/10.1016/j.eswa.2023.121502)  
  *2023 · Forecasting, Decision Control · MultiAgent, RL-Policy, WorldModel · Finance-Trading / Algorithmic Trading / Stock Index Trading*

#### 2024

- [A Multimodal Foundation Agent for Financial Trading: Tool-Augmented, Diversified, and Generalist](https://arxiv.org/pdf/2402.18485) (2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2402.18485)  
  *2024 · Trading · ToolUse, RAG, Self-evolving · Finance-Trading*

- [A Reflective LLM-based Agent to Guide Zero-shot Cryptocurrency Trading](https://arxiv.org/pdf/2407.09546) (2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2407.09546)  
  *2024 · Trading · MultiAgent, Self-evolving · Finance-Trading (Cryptocurrency)*

- [FinCon: A Synthesized LLM Multi-Agent System with Conceptual Verbal Reinforcement for Enhanced Financial Decision Making](https://arxiv.org/pdf/2407.06567) (2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2407.06567)  
  *2024 · Trading, Portfolio Management · MultiAgent, Self-evolving, RL-Policy · Finance-Trading*

- [Open-TI: Open Traffic Intelligence with Augmented Language Model](https://arxiv.org/pdf/2401.00211) (2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2401.00211)  
  *2024 · Traffic Simulation, Signal Control · ToolUse, MultiAgent · Transportation*

- [TradingAgents: Multi-Agents LLM Financial Trading Framework](https://arxiv.org/pdf/2412.20138) (2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2412.20138)  
  *2024 · Trading · MultiAgent, ToolUse · Finance-Trading*

#### 2025

- [ATLAS: Adaptive Trading with LLM AgentS Through Dynamic Prompt Optimization and Multi-Agent Coordination](https://arxiv.org/pdf/2510.15949) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2510.15949)  
  *2025 · Trading · MultiAgent, Self-evolving · Finance-Trading*

- [BRIDGE: Bootstrapping Text to Control Time-Series Generation via Multi-Agent Iterative Optimization and Diffusion Modeling](https://arxiv.org/pdf/2503.02445) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2503.02445)  
  *2025 · Generation · MultiAgent, ReAct · General/Cross-domain*

- [FinArena: A Human-Agent Collaboration Framework for Financial Market Analysis and Forecasting](https://arxiv.org/pdf/2503.02692) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2503.02692)  
  *2025 · Forecasting, Trading · MultiAgent, RAG · Finance-Trading*

- [FinHEAR: Human Expertise and Adaptive Risk-Aware Temporal Reasoning for Financial Decision-Making](https://arxiv.org/pdf/2506.09080) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2506.09080)  
  *2025 · Forecasting · MultiAgent, RAG, ProcMem, Self-evolving · Finance-Trading*

- [Hi-DARTS: Hierarchical Dynamically Adapting Reinforcement Trading System](https://arxiv.org/pdf/2509.12048) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2509.12048)  
  *2025 · Forecasting, Generation · MultiAgent, RL-Policy · Finance-Trading*

- [Integrating Traditional Technical Analysis with AI: A Multi-Agent LLM-Based Approach to Stock Market Forecasting](https://arxiv.org/pdf/2506.16813) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2506.16813)  
  *2025 · Forecasting · MultiAgent, RAG, RL-Policy, ToolUse, ReAct · Finance-Trading*

- [R&D-Agent-Quant: A Multi-Agent Framework for Data-Centric Factors and Model Joint Optimization](https://arxiv.org/pdf/2505.15155) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2505.15155)  
  *2025 · Forecasting · D*

#### 2026

- [AegisTS: A Hierarchical Agent System with Reinforcement Learning for Multivariate Time Series Data Cleaning](https://arxiv.org/pdf/2605.04902) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2605.04902)  
  *2026 · Anomaly Detection, Imputation · RL-Policy, AutoML*

- [AgriWorld: A World Tools Protocol Framework for Verifiable Agricultural Reasoning with Code-Executing LLM Agents](https://arxiv.org/pdf/2602.15325) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2602.15325)  
  *2026 · Forecasting, Anomaly Detection, QA-Reasoning · ToolUse, ReAct, Self-evolving · Agriculture*

- [AION: Next-Generation Tasks and Practical Harness for Time Series](https://arxiv.org/abs/2605.25045) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2605.25045)  
  *2026 · Forecasting · MultiAgent/ToolUse/ReAct/RAG/ProcMem*

- [AIVV: Neuro-Symbolic LLM Agent-Integrated Verification and Validation for Trustworthy Autonomous Systems](https://arxiv.org/pdf/2604.02478) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2604.02478)  
  *2026 · Anomaly Detection, Verification & Validation · MultiAgent, Self-evolving · Autonomous Systems (UUV)*

- [Chronicle: A Multimodal Foundation Model for Joint Language and Time Series Understanding](https://arxiv.org/pdf/2605.20268) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2605.20268)  
  *2026 · Forecasting, Classification, QA*

- [Hubble: An LLM-Driven Agentic Framework for Safe, Diverse, and Reproducible Alpha Factor Discovery](https://arxiv.org/pdf/2604.09601) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2604.09601)  
  *2026 · Alpha Factor Discovery (Trading) · RAG, ToolUse, AutoML · Finance-Trading*

- [SEA-TS: Self-Evolving Agent for Autonomous Code Generation of Time Series Forecasting Algorithms](https://arxiv.org/pdf/2603.04873v1) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2603.04873)  
  *2026 · Forecasting · AutoML, Self-evolving, ProcMem · Energy*

- [Time Series Augmented Generation for Financial Applications](https://arxiv.org/pdf/2604.19633) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2604.19633)  
  *2026 · QA-Reasoning · ToolUse · Finance-Trading*

#### Year Unknown / To Be Checked

- [Multi-Agent Deep RL for Demand Forecasting](https://www.mdpi.com/1424-8220/25/8/2428)  
  [![Paper](https://img.shields.io/badge/Paper-Link-blue.svg)](https://www.mdpi.com/1424-8220/25/8/2428)  
  *Forecasting, Decision Control · MultiAgent, RL-Policy, WorldModel · Retail Supply Chain / Inventory Optimization / Sensor-enabled Retail*

- [StockAgent: A Multi-Agent Collaborative Framework for Financial Time Series Prediction](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=11327922&tag=1)  
  [![IEEE](https://img.shields.io/badge/IEEE-Xplore-00629B.svg)](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=11327922&tag=1)  
  *Decision Control, Energy Trading, Optimization · MultiAgent, RAG, ToolUse, RL-Policy, WorldModel · Smart Grid / Real-time P2P Energy Trading / Distribution Network Operation*

- [TS-GYM: Dynamic Ensemble via Deep RL](https://openreview.net/pdf?id=a6NvoZ5DLoe)  
  [![OpenReview](https://img.shields.io/badge/OpenReview-8c1b13.svg)](https://openreview.net/pdf?id=a6NvoZ5DLoe)  
  *Forecasting · RL-Policy, WorldModel, AutoML*


## Reliability, Safety and Trustworthiness

A cross-cutting subset of works that are especially relevant to evaluation, robustness, grounding, safety, security, auditability, anomaly reasoning, or trustworthy deployment.

### 2023

- [One Fits All: Power General Time Series Analysis by Pretrained LM](https://arxiv.org/pdf/2302.11939) (2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2302.11939)  
  *2023 · Anomaly Detection,Classification,Forecasting,Imputation*

- [TEST: Text Prototype Aligned Embedding to Activate LLM's Ability for Time Series](https://arxiv.org/pdf/2308.08241) (2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2308.08241)  
  *2023 · Forecasting, Classification, Anomaly Detection*

### 2024

- [(CiK) Context is Key: A Benchmark for Forecasting with Essential Textual Information](https://arxiv.org/pdf/2410.18959) (2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2410.18959)  
  *2024 · Forecasting*

- [Agentic Retrieval-Augmented Generation for Time Series Analysis](https://arxiv.org/pdf/2408.14484) (2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2408.14484)  
  *2024 · Forecasting, Anomaly Detection, Classification, Imputation · MultiAgent, RAG, ReAct*

- [Can LLMs Serve as Time Series Anomaly Detectors?](https://arxiv.org/pdf/2408.03475) (2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2408.03475)  
  *2024 · Anomaly Detection*

- [Can LLMs Understand Time Series Anomalies?](https://arxiv.org/pdf/2410.05440) (2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2410.05440)  
  *2024 · Anomaly Detection*

- [Evaluating Large Language Models on Time Series Feature Understanding: A Comprehensive Taxonomy and Benchmark](https://arxiv.org/pdf/2404.16563) (2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2404.16563)  
  *2024 · Classification & QA*

- [Language Models Still Struggle to Zero-shot Reason about Time Series](https://arxiv.org/pdf/2404.11757) (2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2404.11757)  
  *2024 · QA-Reasoning, Forecasting*

- [LEMMA-RCA: A Large Multi-modal Multi-domain Dataset for Root Cause Analysis](https://arxiv.org/pdf/2406.05375) (2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2406.05375)  
  *2024 · Forecasting · IT & IoT*

- [MOMENT: A Family of Open Time-series Foundation Models](https://arxiv.org/pdf/2402.03885) (2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2402.03885)  
  *2024 · Forecasting, Classification, Anomaly Detection, Imputation*

- [TimeSeriesExam: A time series understanding exam](https://arxiv.org/pdf/2410.14752) (2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2410.14752)  
  *2024 · QA & Anomaly Detection & Classification*

- [Toto](https://arxiv.org/pdf/2407.07874) (2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2407.07874)  
  *2024 · Forecasting*

- [TS-Reasoner: Domain-Oriented Time Series Inference Agents for Reasoning and Automated Analysis](https://arxiv.org/pdf/2410.04047) (2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2410.04047)  
  *2024 · Forecasting, Anomaly Detection, QA-Reasoning, Classification · ToolUse, ReAct*

- [UniTS: Building a Unified Time Series Model](https://arxiv.org/pdf/2403.00131) (2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2403.00131)  
  *2024 · Forecasting, Classification, Anomaly Detection, Imputation*

### 2025

- [(EngineMT-QA) ITFormer: Bridging Time Series and Natural Language for Multi-Modal QA with Large-Scale Multitask Dataset](https://arxiv.org/pdf/2506.20093) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2506.20093)  
  *2025 · QA · Aero*

- [A Survey of Reasoning and Agentic Systems in Time Series with Large Language Models](https://arxiv.org/pdf/2509.11575) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2509.11575)  
  *2025 · Forecasting, Anomaly Detection, Classification, QA-Reasoning, Causal Inferenc... · ToolUse, ReAct, RAG, MultiAgent, RL-Policy, Self-evolving*

- [Achieving Time Series Reasoning Requires Rethinking Model Design, Tasks Formulation, and Evaluation](https://arxiv.org/pdf/2502.01477) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2502.01477)  
  *2025 · QA & Forecasting & Classification*

- [AD-AGENT: A Multi-agent Framework for End-to-end Anomaly Detection](https://arxiv.org/pdf/2505.12594) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2505.12594)  
  *2025 · Anomaly Detection · MultiAgent, ToolUse, RAG, AutoML*

- [Argos: Agentic Time-Series Anomaly Detection with Autonomous Rule Generation via LLMs](https://arxiv.org/pdf/2501.14170) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2501.14170)  
  *2025 · Anomaly Detection · MultiAgent, AutoML · Cloud Infrastructure Monitoring (AIOps)*

- [AXIS: Explainable Time Series Anomaly Detection with Large Language Models](https://arxiv.org/pdf/2509.24378) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2509.24378)  
  *2025 · Anomaly Detection*

- [CALM: Continuous, Adaptive, and LLM-Mediated Anomaly Detection in Time-Series Streams](https://arxiv.org/pdf/2508.21273) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2508.21273)  
  *2025 · Anomaly Detection · Self-evolving, AutoML*

- [Can Multimodal LLMs Perform Time Series Anomaly Detection?](https://arxiv.org/pdf/2502.17812) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2502.17812)  
  *2025 · Anomaly Detection · MultiAgent, ToolUse*

- [Chain-of-thought Reviewing and Correction for Time Series Question Answering](https://arxiv.org/pdf/2512.22627) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2512.22627)  
  *2025 · QA · A: 时序数据文本化后输入LLM保留原始数值尺度信息(Sec 2); B: Worker LLM生成结构化逐步CoT推理链(Sec 2.1); Revie...*

- [Fidel-TS: A High-Fidelity Multimodal Benchmark for Time Series Forecasting](https://arxiv.org/pdf/2509.24789) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2509.24789)  
  *2025 · Forecasting*

- [FinHEAR: Human Expertise and Adaptive Risk-Aware Temporal Reasoning for Financial Decision-Making](https://arxiv.org/pdf/2506.09080) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2506.09080)  
  *2025 · Forecasting · MultiAgent, RAG, ProcMem, Self-evolving · Finance-Trading*

- [GEM: Empowering MLLM for Grounded ECG Understanding with Time Series and Images](https://arxiv.org/pdf/2503.06073) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2503.06073)  
  *2025 · Classification & QA · A: 双编码器架构——ECG时间序列编码器(ECG-CoCa预训练)与ECG图像编码器(CLIP from LLaVA)分别提取特征(Sec 3.2); ...*

- [GTM: A General Time-series Model for Enhanced Representation Learning of Time-Series Data](https://arxiv.org/pdf/2502.03264) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2502.03264)  
  *2025 · Forecasting, Classification, Anomaly Detection, Imputation*

- [Hierarchical AI-Meteorologist: LLM-Agent System for Multi-Scale and Explainable Weather Forecast Reporting](https://arxiv.org/pdf/2511.23387) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2511.23387)  
  *2025 · Forecasting · MultiAgent · Weather/Climate*

- [Human in the Loop Adaptive Optimization for Improved Time Series Forecasting](https://arxiv.org/pdf/2505.15354) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2505.15354)  
  *2025 · Forecasting*

- [MERIT: Multi-Agent Collaboration for Unsupervised Time Series Representation Learning](https://aclanthology.org/2025.findings-acl.1231.pdf) (2025)  
  [![Paper](https://img.shields.io/badge/Paper-Link-blue.svg)](https://aclanthology.org/2025.findings-acl.1231.pdf)  
  *2025 · Classification, Forecasting, Anomaly Detection, Transfer Learning, Representa... · MultiAgent, RAG, ProcMem*

- [R&D-Agent-Quant: A Multi-Agent Framework for Data-Centric Factors and Model Joint Optimization](https://arxiv.org/pdf/2505.15155) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2505.15155)  
  *2025 · Forecasting · D*

- [Time Series Forecasting as Reasoning: A Slow-Thinking Approach with Reinforced LLMs](https://arxiv.org/pdf/2506.10630) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2506.10630)  
  *2025 · Forecasting · RL-Policy*

- [Time-MQA](https://arxiv.org/pdf/2503.01875) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2503.01875)  
  *2025 · Forecasting, Imputation, Anomaly Detection, Classification, QA*

- [TIME-RA: Towards Time Series Reasoning for Anomaly Diagnosis with LLM Feedback](https://arxiv.org/pdf/2507.15066) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2507.15066)  
  *2025 · Anomaly Detection, Classification, QA-Reasoning*

- [TimeSeriesGym: A Scalable Benchmark for (Time Series) Machine Learning Engineering Agents](https://arxiv.org/pdf/2505.13291) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2505.13291)  
  *2025 · Forecasting, Classification, Anomaly Detection, QA-Reasoning, Regression, Imp...*

- [Towards Interpretable and Trustworthy Time Series Reasoning: A BlueSky Vision](https://arxiv.org/pdf/2510.16980) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2510.16980)  
  *2025 · Forecasting & QA & Anomaly Detection & Classification*

- [Trading-R1: Financial Trading with LLM Reasoning via Reinforcement Learning](https://arxiv.org/pdf/2509.11420) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2509.11420)  
  *2025 · Forecasting & Classification · A: 多模态感知——整合技术市场数据(价格/EMA/波动率)/基本面数据/新闻/内部人情绪/宏观经济指标等多源异构金融信息(Sec 3.2); B: 结构...*

- [TS-Agent: A Time Series Reasoning Agent with Iterative Statistical Insight Gathering (ReAct-style)](https://arxiv.org/pdf/2510.07432) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2510.07432)  
  *2025 · Anomaly Detection, Classification, QA-Reasoning · ReAct, ToolUse*

- [TS-Reasoner: Aligning Time Series Foundation Models with LLM Reasoning](https://arxiv.org/pdf/2510.03519) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2510.03519)  
  *2025 · QA & Classification · A: 使用冻结的预训练TSFM(TimesFM)编码patched时序为紧凑嵌入，再通过MLP适配器投影到LLM输入嵌入空间(Sec 3.1); B: 通...*

- [TSPulse: Tiny Pre-Trained Models with Disentangled Representations for Rapid Time-Series Analysis](https://arxiv.org/pdf/2505.13033) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2505.13033)  
  *2025 · Classification, Anomaly Detection, Imputation, Similarity Search*

- [When LLM Meets Time Series: Can LLMs Perform Multistep Time Series Reasoning and Inference](https://arxiv.org/pdf/2509.01822) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2509.01822)  
  *2025 · Forecasting, Anomaly Detection, QA-Reasoning, Classification · General/Energy/Climate/Finance/Healthcare*

- [ZARA: Training-Free Motion Time-Series Reasoning via Evidence-Grounded LLM Agents](https://arxiv.org/pdf/2508.04038) (2025)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2508.04038)  
  *2025 · Classification · RAG, MultiAgent, CoT · General (Human Activity Recognition)*

### 2026

- [AegisTS: A Hierarchical Agent System with Reinforcement Learning for Multivariate Time Series Data Cleaning](https://arxiv.org/pdf/2605.04902) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2605.04902)  
  *2026 · Anomaly Detection, Imputation · RL-Policy, AutoML*

- [Agentic Trading: When LLM Agents Meet Financial Markets](https://arxiv.org/pdf/2605.19337) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2605.19337)  
  *2026 · Forecasting, Anomaly Detection, Classification · ToolUse, ReAct, RAG, MultiAgent, RL-Policy, Self-evolving · Finance-Trading*

- [AgriWorld: A World Tools Protocol Framework for Verifiable Agricultural Reasoning with Code-Executing LLM Agents](https://arxiv.org/pdf/2602.15325) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2602.15325)  
  *2026 · Forecasting, Anomaly Detection, QA-Reasoning · ToolUse, ReAct, Self-evolving · Agriculture*

- [AIVV: Neuro-Symbolic LLM Agent-Integrated Verification and Validation for Trustworthy Autonomous Systems](https://arxiv.org/pdf/2604.02478) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2604.02478)  
  *2026 · Anomaly Detection, Verification & Validation · MultiAgent, Self-evolving · Autonomous Systems (UUV)*

- [AnomaMind: Agentic Time Series Anomaly Detection with Tool-Augmented Reasoning](https://arxiv.org/pdf/2602.13807) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2602.13807)  
  *2026 · Anomaly Detection · ToolUse, ReAct, RL-Policy*

- [ChatAD: Reasoning-Enhanced Time-Series Anomaly Detection with Multi-Turn Instruction Evolution](https://arxiv.org/pdf/2601.13546) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2601.13546)  
  *2026 · Anomaly Detection,Classification,Imputation · MultiAgent, Self-evolving, ProcMem · General / Anomaly Detection*

- [Dr-CiK: A Testbed for Foresight-Driven Agents](https://arxiv.org/pdf/2605.27904) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2605.27904)  
  *2026 · Forecasting*

- [Foresight Arena: An On-Chain Benchmark for Evaluating AI Forecasting Agents](https://arxiv.org/pdf/2605.00420) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2605.00420)  
  *2026 · Forecasting · ToolUse, Benchmark, On-chain Verification · General/Prediction Markets*

- [HEARTS: Benchmarking LLM Reasoning on Health Time Series](https://arxiv.org/pdf/2603.06638) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2603.06638)  
  *2026 · Classification & Forecasting & Imputation & QA · Health*

- [Hubble: An LLM-Driven Agentic Framework for Safe, Diverse, and Reproducible Alpha Factor Discovery](https://arxiv.org/pdf/2604.09601) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2604.09601)  
  *2026 · Alpha Factor Discovery (Trading) · RAG, ToolUse, AutoML · Finance-Trading*

- [It's TIME: Towards the Next Generation of Time Series Forecasting Benchmarks](https://arxiv.org/pdf/2602.12147) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2602.12147)  
  *2026 · Forecasting*

- [LLM-Enhanced Reinforcement Learning for Time Series Anomaly Detection](https://arxiv.org/pdf/2601.02511) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2601.02511)  
  *2026 · Anomaly Detection · RL-Policy*

- [Rationale-Grounded In-Context Learning for Time Series Reasoning with Multimodal Large Language Models](https://arxiv.org/pdf/2601.02968) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2601.02968)  
  *2026 · Classification · A: MLLM接收时序可视化图表作为视觉输入(Sec 3.2); TabPFN编码器提取时序数据嵌入用于数据驱动检索(Sec 3.2); 文本嵌入模型编码...*

- [Reasoning through Verifiable Forecast Actions: Consistency-Grounded RL for Financial LLMs](https://arxiv.org/pdf/2605.21975) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2605.21975)  
  *2026 · Forecasting/QA · ToolUse/RL-Policy*

- [SAGE: Detecting Time Series Anomalies Like an Expert: A Multi-Agent LLM Framework with Specialized Analyzers](https://arxiv.org/pdf/2605.05725) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2605.05725)  
  *2026 · Anomaly Detection · MultiAgent, ToolUse, RAG*

- [TemporalBench: A Benchmark for Evaluating LLM-Based Agents on Contextual and Event-Informed Time Series Tasks](https://arxiv.org/pdf/2602.13272) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2602.13272)  
  *2026 · Forecasting, QA, Anomaly Detection*

- [TFRBench: A Reasoning Benchmark for Evaluating Forecasting Systems](https://arxiv.org/pdf/2604.05364) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2604.05364)  
  *2026 · Forecasting*

- [Time Series Augmented Generation for Financial Applications](https://arxiv.org/pdf/2604.19633) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2604.19633)  
  *2026 · QA-Reasoning · ToolUse · Finance-Trading*

- [Time Series Reasoning via Process-Verifiable Thinking Data Synthesis and Scheduling for Tailored LLM Reasoning](https://arxiv.org/pdf/2602.07830) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2602.07830)  
  *2026 · QA-Reasoning, Anomaly Detection, Classification · RL-Policy*

- [TimeSeriesExamAgent](https://arxiv.org/pdf/2604.10291) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2604.10291)  
  *2026 · QA, Anomaly Detection*

- [TSRBench: A Comprehensive Multi-task Multi-modal Time Series Reasoning Benchmark for Generalist Models](https://arxiv.org/pdf/2601.18744) (2026)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2601.18744)  
  *2026 · Forecasting, Anomaly Detection, QA-Reasoning, Classification*

### Year Unknown / To Be Checked

- [An Interpretable Agent-Assisted Pipeline for Statistical Anomaly Detection in IoT Temperature Time Series](https://www.mdpi.com/2079-9292/15/9/1840)  
  [![Paper](https://img.shields.io/badge/Paper-Link-blue.svg)](https://www.mdpi.com/2079-9292/15/9/1840)  
  *Anomaly Detection · Rule-based Agent-Assisted Selection · IoT / Edge Monitoring / Temperature Sensor Anomaly Detection*

- [AutoLM](https://link.springer.com/content/pdf/10.1007/s12273-025-1385-7.pdf)  
  [![Springer](https://img.shields.io/badge/Springer-Link-6db33f.svg)](https://link.springer.com/content/pdf/10.1007/s12273-025-1385-7.pdf)  
  *Forecasting · MultiAgent, RAG, AutoML, ToolUse · Building Energy / Load Forecasting / Smart Building*

- [Delving into Large Language Models for Effective Time-Series Anomaly Detection](https://openreview.net/pdf?id=6rpy7X1Of8)  
  [![OpenReview](https://img.shields.io/badge/OpenReview-8c1b13.svg)](https://openreview.net/pdf?id=6rpy7X1Of8)  
  *Anomaly Detection · A: 系统比较多种时序表示方法(原始数值序列/tokenization离散化/patch编码等)将时序信号输入LLM的方式研究不同表示对异常检测效果的影响...*

- [From Prompts to Agents: A Comprehensive Survey of LLM-Driven Time Series Analysis](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=6614598)  
  [![Paper](https://img.shields.io/badge/Paper-Link-blue.svg)](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=6614598)  
  *Forecasting, Anomaly Detection, Classification, Imputation, QA-Reasoning · ToolUse, RAG, MultiAgent, Self-evolving/Reflection*

- [LLM Agents Struggle at Engineering Time Series Solutions](https://openreview.net/pdf?id=04fwpztRMB)  
  [![OpenReview](https://img.shields.io/badge/OpenReview-8c1b13.svg)](https://openreview.net/pdf?id=04fwpztRMB)  
  *Forecasting, Anomaly Detection, Classification, Imputation, Time Series Under... · AutoML, ToolUse, ReAct (注：评测对象如 AIDE, OpenHands 均依赖于 ToolUse/CodeAct 交互模式，且任务...*

- [MAS-LSTM: A Multi-Agent LSTM-Based Approach for Scalable Anomaly Detection in IIoT Networks](https://www.scilit.com/publications/mas-lstm)  
  [![Paper](https://img.shields.io/badge/Paper-Link-blue.svg)](https://www.scilit.com/publications/mas-lstm)  
  *Anomaly Detection · MultiAgent · Industrial IoT / Network Security / Intrusion & Anomaly Detection*

- [Multi-Agent Adversarial Time Series Forecasting](https://openreview.net/forum?id=lj1qwU6Gxs)  
  [![OpenReview](https://img.shields.io/badge/OpenReview-8c1b13.svg)](https://openreview.net/forum?id=lj1qwU6Gxs)  
  *Forecasting · MultiAgent, RL-Policy · Finance-Trading, General*

- [TS-GYM: Dynamic Ensemble via Deep RL](https://openreview.net/pdf?id=a6NvoZ5DLoe)  
  [![OpenReview](https://img.shields.io/badge/OpenReview-8c1b13.svg)](https://openreview.net/pdf?id=a6NvoZ5DLoe)  
  *Forecasting · RL-Policy, WorldModel, AutoML*


## Contributing

We welcome contributions. Please open an issue or pull request if you would like to:

- add a missing paper, dataset, benchmark, codebase, or survey;
- correct a paper title, link, year, category, or tag;
- add project pages, code links, venues, or BibTeX entries;
- suggest a better taxonomy for agentic time series systems.

Suggested pull request format:

```markdown
- [Paper Title](paper_link) (Year)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](arxiv_link)
  *Task / Mechanism / Domain tags*
```

## Citation

If you find this repository useful, please consider citing the associated survey:

```bibtex

```

## License

This repository is released under the MIT License. The papers, datasets, and external resources remain under their original licenses.
