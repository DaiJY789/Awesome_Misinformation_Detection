<h1 id="awesome-misinformation-detection-in-the-aigc-era" align="center">Awesome Misinformation Detection in the AIGC Era</h1>

<p align="center">
  <img src="https://img.shields.io/badge/Status-Submitted%20to%20TKDE-00629B.svg" alt="Submitted to TKDE">
  <a href="https://github.com/zeng-yirong/Awesome_Misinformation_Detection/stargazers"><img src="https://img.shields.io/github/stars/zeng-yirong/Awesome_Misinformation_Detection?style=social" alt="Stars"></a>
  <a href="https://github.com/zeng-yirong/Awesome_Misinformation_Detection/network/members"><img src="https://img.shields.io/github/forks/zeng-yirong/Awesome_Misinformation_Detection?style=social" alt="Forks"></a>
  <a href="https://github.com/zeng-yirong/Awesome_Misinformation_Detection/issues"><img src="https://img.shields.io/github/issues/zeng-yirong/Awesome_Misinformation_Detection" alt="Issues"></a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Phase%20I-Pre--LLM%20MID-4C78A8" alt="Phase I">
  <img src="https://img.shields.io/badge/Phase%20II-LLM--Augmented%20MID-54A24B" alt="Phase II">
  <img src="https://img.shields.io/badge/Phase%20III-AIGC--era%20MID-E45756" alt="Phase III">
  <img src="https://img.shields.io/badge/Benchmark-Evaluation%20Resources-F2CF5B" alt="Benchmark">
</p>

<p align="center">
  This is the official repository for the survey paper:<br>
  <strong>Misinformation Detection in the AIGC Era: Methods, Benchmarks, and Challenges</strong><br>
  Juyi Dai, Yirong Zeng, Xiao Ding, Jiashun Luo, Bibo Cai, Shen You, Wenyu Zang, Bing Qin, and Ting Liu<br>
  <em>Research Center for Social Computing and Interactive Robotics, Harbin Institute of Technology</em><br>
  Corresponding author: Xiao Ding
</p>

We maintain a structured reading list of method and system papers cited in the survey, tracing misinformation detection (MID) from pre-LLM data-driven methods to LLM-augmented verification and AIGC-era challenges. Within each subsection, papers are sorted by publication year in ascending order and alphabetically by original title within the same year. Formal conference or journal versions are used whenever confirmed; entries are labeled arXiv only when no formal version was found. Surveys, audits, datasets, and purely analytical studies are excluded from method subsections, while datasets and evaluation resources cited in the survey are collected separately under Benchmark.

---

<h2 id="introduction">🌟 Introduction</h2>

Misinformation detection (MID) is being reshaped by the rapid development of AI-generated content (AIGC). Large language models (LLMs) and multi-modal generative models play a dual role: they strengthen verification through reasoning, retrieval, and multi-modal understanding, while also lowering the cost of producing persuasive false or misleading content.

This survey provides an evolutionary view of MID in the AIGC era. Rather than reviewing isolated tasks or methods, we organize the field into three phases: **Pre-LLM MID**, **LLM-Augmented MID**, and **AIGC-era MID**. We further clarify the conceptual scope of misinformation and MID, review benchmark and evaluation evolution, and outline future directions including agentic verification, lifelong detection, and unified systems.

<p align="center">
  <img src="img/Evo.png" width="100%" alt="Evolutionary Taxonomy of MID">
</p>

<h2 id="news">📰 News</h2>

- **2026-07-15:** Our survey paper, **Misinformation Detection in the AIGC Era: Methods, Benchmarks, and Challenges**, was submitted to *IEEE Transactions on Knowledge and Data Engineering (TKDE)*.

---

<h2 id="contents">📚 Contents</h2>

<details open>
<summary>📚 Contents</summary>

- [Awesome Misinformation Detection in the AIGC Era](#awesome-misinformation-detection-in-the-aigc-era)
  - [🌟 Introduction](#introduction)
  - [📰 News](#news)
  - [📚 Contents](#contents)
  - [🧱 Phase I: Pre-LLM MID](#phase-i-pre-llm-mid)
    - [Content-based](#content-based)
    - [Context-based](#context-based)
    - [Evidence-based](#evidence-based)
    - [Cross-modal](#cross-modal)
  - [🤖 Phase II: LLM-Augmented MID](#phase-ii-llm-augmented-mid)
    - [Reasoning](#reasoning)
    - [Retrieval](#retrieval)
    - [Simulation](#simulation)
    - [Multimodal](#multimodal)
  - [✨ Phase III: AIGC-era MID](#phase-iii-aigc-era-mid)
    - [AI-generated Fabrication](#ai-generated-fabrication)
    - [Misinformative Hallucinations](#misinformative-hallucinations)
    - [Multimedia Deepfake](#multimedia-deepfake)
  - [📊 Benchmark](#benchmark)
  - [🚀 Future Direction](#future-direction)
    - [Agentic Verification](#agentic-verification)
    - [Lifelong Detection](#lifelong-detection)
    - [Unified System](#unified-system)
  - [✍️ Citation](#citation)

</details>

---

<h2 id="phase-i-pre-llm-mid">🧱 Phase I: Pre-LLM MID</h2>

Pre-LLM MID mainly targets human-authored misinformation and learns detection signals from content, social context, external evidence, and cross-modal consistency.

<h3 id="content-based">Content-based</h3>

- **LUX (Linguistic Aspects Under Examination): Discourse Analysis for Automatic Fake News Classification**. Findings of ACL, 2021. [[paper](https://aclanthology.org/2021.findings-acl.4/)]
- **Demystifying Neural Fake News via Linguistic Feature-Based Interpretation**. COLING, 2022. [[paper](https://aclanthology.org/2022.coling-1.576/)]
- **Linguistic Features Based Framework for Automatic Fake News Detection**. Computers & Industrial Engineering, 2022. [[paper](https://doi.org/10.1016/j.cie.2022.108432)]
- **Bridging Thoughts and Words: Graph-Based Intent-Semantic Joint Learning for Fake News Detection**. CIKM, 2025. [[paper](https://doi.org/10.1145/3746252.3761400)]
- **Graph with Sequence: Broad-Range Semantic Modeling for Fake News Detection**. WWW, 2025. [[paper](https://doi.org/10.1145/3696410.3714906)]

<h3 id="context-based">Context-based</h3>

- **Beyond News Contents: The Role of Social Context for Fake News Detection**. WSDM, 2019. [[paper](https://doi.org/10.1145/3289600.3290994)]
- **Rumor Detection on Social Media with Bi-Directional Graph Convolutional Networks**. AAAI, 2020. [[paper](https://doi.org/10.1609/aaai.v34i01.5393)]
- **Zoom Out and Observe: News Environment Perception for Fake News Detection**. ACL, 2022. [[paper](https://aclanthology.org/2022.acl-long.311/)]
- **A Macro-and Micro-Hierarchical Transfer Learning Framework for Cross-Domain Fake News Detection**. WWW, 2025. [[paper](https://doi.org/10.1145/3696410.3714517)]
- **Variety Is the Spice of Life: Detecting Misinformation with Dynamic Environmental Representations**. CIKM, 2025. [[paper](https://doi.org/10.1145/3746252.3761114)]

<h3 id="evidence-based">Evidence-based</h3>

- **Compare to the Knowledge: Graph Neural Fake News Detection with External Knowledge**. ACL, 2021. [[paper](https://aclanthology.org/2021.acl-long.62/)]
- **FACE-KEG: Fact Checking Explained Using Knowledge Graphs**. WSDM, 2021. [[paper](https://doi.org/10.1145/3437963.3441828)]
- **Incorporating Relational Knowledge in Explainable Fake News Detection**. PAKDD, 2021. [[paper](https://doi.org/10.1007/978-3-030-75768-7_32)]
- **KAN: Knowledge-Aware Attention Network for Fake News Detection**. AAAI, 2021. [[paper](https://doi.org/10.1609/aaai.v35i1.16080)]
- **Generating Literal and Implied Subquestions to Fact-Check Complex Claims**. EMNLP, 2022. [[paper](https://aclanthology.org/2022.emnlp-main.229/)]
- **Towards Fine-Grained Reasoning for Fake News Detection**. AAAI, 2022. [[paper](https://doi.org/10.1609/aaai.v36i5.20517)]
- **Claim-Dissector: An Interpretable Fact-Checking System with Joint Re-Ranking and Veracity Prediction**. Findings of ACL, 2023. [[paper](https://aclanthology.org/2023.findings-acl.647/)]
- **FactKG: Fact Verification via Reasoning on Knowledge Graphs**. ACL, 2023. [[paper](https://aclanthology.org/2023.acl-long.895/)]
- **Fact or Fiction? Improving Fact Verification with Knowledge Graphs through Simplified Subgraph Retrievals**. FEVER, 2024. [[paper](https://aclanthology.org/2024.fever-1.32/)]

<h3 id="cross-modal">Cross-modal</h3>

- **Hierarchical Multi-Modal Contextual Attention Network for Fake News Detection**. SIGIR, 2021. [[paper](https://doi.org/10.1145/3404835.3462871)]
- **InfoSurgeon: Cross-Media Fine-Grained Information Consistency Checking for Fake News Detection**. ACL, 2021. [[paper](https://aclanthology.org/2021.acl-long.133/)]
- **Unseen Fake News Detection Through Causal Debiasing**. WWW Companion, 2025. [[paper](https://doi.org/10.1145/3701716.3715517)]

---

<h2 id="phase-ii-llm-augmented-mid">🤖 Phase II: LLM-Augmented MID</h2>

LLMs augment existing MID pipelines through reasoning, retrieval, context reconstruction, and multi-modal understanding.

<h3 id="reasoning">Reasoning</h3>

- **TELLER: A Trustworthy Framework for Explainable, Generalizable and Controllable Fake News Detection**. Findings of ACL, 2024. [[paper](https://aclanthology.org/2024.findings-acl.919/)]
- **PCoT: Persuasion-Augmented Chain of Thought for Detecting Fake News and Social Media Disinformation**. ACL, 2025. [[paper](https://aclanthology.org/2025.acl-long.1215/)]
- **Towards Real-Time Fake News Detection under Evidence Scarcity**. arXiv, 2025. [[paper](https://arxiv.org/abs/2510.11277)]
- **A Graph-Enhanced Defense Framework for Explainable Fake News Detection with LLM**. ACM TOIS, 2026. [[paper](https://doi.org/10.1145/3810244)]
- **FactGuard: Event-Centric and Commonsense-Guided Fake News Detection**. AAAI, 2026. [[paper](https://doi.org/10.1609/aaai.v40i1.36998)]
- **KG-CRAFT: Knowledge Graph-based Contrastive Reasoning with LLMs for Enhancing Automated Fact-checking**. EACL, 2026. [[paper](https://aclanthology.org/2026.eacl-long.302/)]
- **Reasoning About the Unsaid: Misinformation Detection with Omission-Aware Graph Inference**. AAAI, 2026. [[paper](https://doi.org/10.1609/aaai.v40i2.37097)]

<h3 id="retrieval">Retrieval</h3>

- **Check Your Facts and Try Again: Improving Large Language Models with External Knowledge and Automated Feedback**. arXiv, 2023. [[paper](https://arxiv.org/abs/2302.12813)]
- **FactLLaMA: Optimizing Instruction-Following Language Models with External Knowledge for Automated Fact-Checking**. APSIPA ASC, 2023. [[paper](https://doi.org/10.1109/APSIPAASC58517.2023.10317251)]
- **A Dynamic Knowledge Update-Driven Model with Large Language Models for Fake News Detection**. IJCAI, 2024. [[paper](https://doi.org/10.24963/ijcai.2024/334)]
- **VeraCT Scan: Retrieval-Augmented Fake News Detection with Justifiable Reasoning**. ACL Demo, 2024. [[paper](https://aclanthology.org/2024.acl-demos.25/)]
- **+ VeriRel: Verification Feedback to Enhance Document Retrieval for Scientific Fact Checking**. CIKM, 2025. [[paper](https://doi.org/10.1145/3746252.3760822)]
- **FIRE: Fact-Checking with Iterative Retrieval and Verification**. Findings of NAACL, 2025. [[paper](https://aclanthology.org/2025.findings-naacl.158/)]
- **HiEAG: Evidence-Augmented Generation for Out-of-Context Misinformation Detection**. arXiv, 2025. [[paper](https://arxiv.org/abs/2511.14027)]
- **When Retrieval Outperforms Generation: Dense Evidence Retrieval for Scalable Fake News Detection**. LDK, 2025. [[paper](https://aclanthology.org/2025.ldk-1.26/)]
- **REVEAL: Retrieval-Enhanced Verification for Multimodal Fact-Checking**. FEVER, 2026. [[paper](https://aclanthology.org/2026.fever-1.8/)]
- **User-Centric Evidence Ranking for Attribution and Fact Verification**. EACL, 2026. [[paper](https://aclanthology.org/2026.eacl-long.340/)]
- **ZoFia: Zero-Shot Fake News Detection with Entity-Guided Retrieval and Multi-LLM Interaction**. Findings of ACL, 2026. [[paper](https://aclanthology.org/2026.findings-acl.1083/)]

<h3 id="simulation">Simulation</h3>

- **DELL: Generating Reactions and Explanations for LLM-Based Misinformation Detection**. Findings of ACL, 2024. [[paper](https://aclanthology.org/2024.findings-acl.155/)]
- **Let Silence Speak: Enhancing Fake News Detection with Generated Comments from Large Language Models**. CIKM, 2024. [[paper](https://doi.org/10.1145/3627673.3679519)]
- **Do Not Wait: Preemptive Rumor Detection with Cooperative LLMs and Accessible Social Context**. Information Processing & Management, 2025. [[paper](https://doi.org/10.1016/j.ipm.2024.103995)]
- **Exploring Large Language Models for Effective Rumor Detection on Social Media**. NAACL, 2025. [[paper](https://aclanthology.org/2025.naacl-long.128/)]
- **Group-Adaptive Adversarial Learning for Robust Fake News Detection Against Malicious Comments**. arXiv, 2025. [[paper](https://arxiv.org/abs/2510.09712)]
- **MPCG: Multi-Round Persona-Conditioned Generation for Modeling the Evolution of Misinformation with LLMs**. EMNLP, 2025. [[paper](https://aclanthology.org/2025.emnlp-main.1727/)]
- **Simulating Rumor Spreading in Social Networks Using LLM Agents**. arXiv, 2025. [[paper](https://arxiv.org/abs/2502.01450)]
- **Structure-Aware Propagation Generation with Large Language Models for Fake News Detection**. Findings of EMNLP, 2025. [[paper](https://aclanthology.org/2025.findings-emnlp.714/)]
- **Synergizing LLMs with Global Label Propagation for Multimodal Fake News Detection**. ACL, 2025. [[paper](https://aclanthology.org/2025.acl-long.72/)]
- **CLEAR: Prototype-Conditioned Flow Purification for LLM-Based Rumor Detection with Dirichlet Evidential Learning**. Information Processing & Management, 2026. [[paper](https://doi.org/10.1016/j.ipm.2026.104887)]

<h3 id="multimodal">Multimodal</h3>

- **SNIFFER: Multimodal Large Language Model for Explainable Out-of-Context Misinformation Detection**. CVPR, 2024. [[paper](https://openaccess.thecvf.com/content/CVPR2024/html/Qi_SNIFFER_Multimodal_Large_Language_Model_for_Explainable_Out-of-Context_Misinformation_Detection_CVPR_2024_paper.html)]
- **DEFAME: Dynamic Evidence-Based Fact-Checking with Multimodal Experts**. ICML, 2025. [[paper](https://proceedings.mlr.press/v267/braun25b.html)]
- **Debunk and Infer: Multimodal Fake News Detection via Diffusion-Generated Evidence and LLM Reasoning**. arXiv, 2025. [[paper](https://arxiv.org/abs/2506.21557)]
- **EXCLAIM: An Explainable Cross-Modal Agentic System for Misinformation Detection with Hierarchical Retrieval**. arXiv, 2025. [[paper](https://arxiv.org/abs/2504.06269)]
- **MERIT: Modular Framework for Multimodal Misinformation Detection with Web-Grounded Reasoning**. arXiv, 2025. [[paper](https://arxiv.org/abs/2510.17590)]
- **Multimodal Fact-Checking with Vision Language Models: A Probing Classifier Based Solution with Embedding Strategies**. COLING, 2025. [[paper](https://aclanthology.org/2025.coling-main.310/)]
- **TRUST-VL: An Explainable News Assistant for General Multimodal Misinformation Detection**. EMNLP, 2025. [[paper](https://aclanthology.org/2025.emnlp-main.284/)]
- **ADOSE: Active Multi-Source Domain Adaptation for Multimodal Fake News Detection**. AAAI, 2026. [[paper](https://doi.org/10.1609/aaai.v40i24.39125)]
- **RAMA: Retrieval-Augmented Multi-Agent Framework for Misinformation Detection in Multimodal Fact-Checking**. WWW Companion, 2026. [[paper](https://doi.org/10.1145/3774905.3796483)]
- **T2Agent: A Tool-Augmented Multimodal Misinformation Detection Agent with Monte Carlo Tree Search**. AAAI, 2026. [[paper](https://doi.org/10.1609/aaai.v40i1.36977)]
- **Toward Multimodal Fake News Detection by Multi-Perspective Rationale Generation and Verification**. AAAI, 2026. [[paper](https://doi.org/10.1609/aaai.v40i1.36965)]

---

<h2 id="phase-iii-aigc-era-mid">✨ Phase III: AIGC-era MID</h2>

AIGC-era MID focuses on detection targets introduced or amplified by generative AI: AI-generated fabrications, deepfakes, and hallucinations.

<h3 id="ai-generated-fabrication">AI-generated Fabrication</h3>

- **Fake News in Sheep's Clothing: Robust Fake News Detection Against LLM-Empowered Style Attacks**. KDD, 2024. [[paper](https://doi.org/10.1145/3637528.3671977)]
- **Adversarial Style Augmentation via Large Language Model for Robust Fake News Detection**. WWW, 2025. [[paper](https://doi.org/10.1145/3696410.3714569)]
- **Attacking Misinformation Detection Using Adversarial Examples Generated by Language Models**. EMNLP, 2025. [[paper](https://aclanthology.org/2025.emnlp-main.1405/)]
- **Debate-to-Detect: Reformulating Misinformation Detection as a Real-World Debate with Large Language Models**. EMNLP, 2025. [[paper](https://aclanthology.org/2025.emnlp-main.764/)]
- **Kill Two Birds with One Stone: Generalized and Robust AI-Generated Text Detection via Dynamic Perturbations**. NAACL, 2025. [[paper](https://aclanthology.org/2025.naacl-long.446/)]
- **MAD-Sherlock: Multi-Agent Debate for Visual Misinformation Detection**. ICML Workshop, 2025. [[paper](https://icml.cc/virtual/2025/47995)]
- **RetrieverGuard: Empowering Information Retrieval to Combat LLM-Generated Misinformation**. Findings of NAACL, 2025. [[paper](https://aclanthology.org/2025.findings-naacl.249/)]
- **The Truth Becomes Clearer Through Debate! Multi-Agent Systems with Large Language Models Unmask Fake News**. SIGIR, 2025. [[paper](https://doi.org/10.1145/3726302.3730092)]
- **Cross-Prompt Generalization in Detecting AI-Generated Fake News Using Interpretable Linguistic Features**. arXiv, 2026. [[paper](https://arxiv.org/abs/2606.04199)]
- **Human vs. Machine Deception: Distinguishing AI-Generated and Human-Written Fake News Using Ensemble Learning**. arXiv, 2026. [[paper](https://arxiv.org/abs/2604.09960)]

<h3 id="misinformative-hallucinations">Misinformative Hallucinations</h3>

- **SelfCheckGPT: Zero-Resource Black-Box Hallucination Detection for Generative Large Language Models**. EMNLP, 2023. [[paper](https://aclanthology.org/2023.emnlp-main.557/)]
- **ReEval: Automatic Hallucination Evaluation for Retrieval-Augmented Large Language Models via Transferable Adversarial Attacks**. Findings of NAACL, 2024. [[paper](https://aclanthology.org/2024.findings-naacl.85/)]
- **Consistency Is the Key: Detecting Hallucinations in LLM Generated Text by Checking Inconsistencies About Key Facts**. Findings of IJCNLP-AACL, 2025. [[paper](https://aclanthology.org/2025.findings-ijcnlp.129/)]
- **HalluciNot: Hallucination Detection Through Context and Common Knowledge Verification**. arXiv, 2025. [[paper](https://arxiv.org/abs/2504.07069)]
- **Zero-Knowledge LLM Hallucination Detection and Mitigation Through Fine-Grained Cross-Model Consistency**. EMNLP Industry Track, 2025. [[paper](https://aclanthology.org/2025.emnlp-industry.139/)]
- **FactSelfCheck: Fact-Level Black-Box Hallucination Detection for LLMs**. Findings of EACL, 2026. [[paper](https://aclanthology.org/2026.findings-eacl.296/)]
- **Hallucination Begins Where Saliency Drops**. ICLR, 2026. [[paper](https://iclr.cc/virtual/2026/oral/10007035)]
- **HalluGuard: Demystifying Data-Driven and Reasoning-Driven Hallucinations in LLMs**. ICLR, 2026. [[paper](https://iclr.cc/virtual/2026/poster/10008801)]
- **PHPFND: Detecting Fake News via Post-Hoc Processing of LLMs Hallucination**. AAAI, 2026. [[paper](https://doi.org/10.1609/aaai.v40i1.37050)]
- **The Energy of Falsehood: Detecting Hallucinations via Diffusion Model Likelihoods**. FEVER, 2026. [[paper](https://aclanthology.org/2026.fever-1.4/)]
- **TruthfulRAG: Resolving Factual-Level Conflicts in Retrieval-Augmented Generation with Knowledge Graphs**. AAAI, 2026. [[paper](https://doi.org/10.1609/aaai.v40i38.40489)]

<h3 id="multimedia-deepfake">Multimedia Deepfake</h3>

- **BusterX: MLLM-Powered AI-Generated Video Forgery Detection and Explanation**. arXiv, 2025. [[paper](https://arxiv.org/abs/2505.12620)]
- **CAD: A General Multimodal Framework for Video Deepfake Detection via Cross-Modal Alignment and Distillation**. arXiv, 2025. [[paper](https://arxiv.org/abs/2505.15233)]
- **D3: Scaling Up Deepfake Detection by Learning from Discrepancy**. CVPR, 2025. [[paper](https://openaccess.thecvf.com/content/CVPR2025/html/Yang_D3_Scaling_Up_Deepfake_Detection_by_Learning_from_Discrepancy_CVPR_2025_paper.html)]
- **FakeShield: Explainable Image Forgery Detection and Localization via Multi-Modal Large Language Models**. ICLR, 2025. [[paper](https://proceedings.iclr.cc/paper_files/paper/2025/hash/4d4e0ab9d8ff180bf5b95c258842d16e-Abstract-Conference.html)]
- **LEGION: Learning to Ground and Explain for Synthetic Image Detection**. ICCV, 2025. [[paper](https://openaccess.thecvf.com/content/ICCV2025/html/Kang_LEGION_Learning_to_Ground_and_Explain_for_Synthetic_Image_Detection_ICCV_2025_paper.html)]
- **SIDA: Social Media Image Deepfake Detection, Localization and Explanation with Large Multimodal Model**. CVPR, 2025. [[paper](https://openaccess.thecvf.com/content/CVPR2025/html/Huang_SIDA_Social_Media_Image_Deepfake_Detection_Localization_and_Explanation_with_CVPR_2025_paper.html)]
- **Spot the Fake: Large Multimodal Model-Based Synthetic Image Detection with Artifact Explanation**. arXiv, 2025. [[paper](https://arxiv.org/abs/2503.14905)]
- **TruthLens: Visual Grounding for Universal DeepFake Reasoning**. arXiv, 2025. [[paper](https://arxiv.org/abs/2503.15867)]
- **PRPO: Paragraph-Level Policy Optimization for Vision-Language Deepfake Detection**. ICML, 2026. [[paper](https://icml.cc/virtual/2026/poster/65679)]
- **Revealing the Truth with ConLLM for Detecting Multi-Modal Deepfakes**. Findings of EACL, 2026. [[paper](https://aclanthology.org/2026.findings-eacl.102/)]
- **TranX-Adapter: Bridging Artifacts and Semantics within MLLMs for Robust AI-Generated Image Detection**. arXiv, 2026. [[paper](https://arxiv.org/abs/2602.21716)]
- **Veritas: Generalizable Deepfake Detection via Pattern-Aware Reasoning**. ICLR, 2026. [[paper](https://iclr.cc/virtual/2026/poster/10011453)]

---

<h2 id="benchmark">📊 Benchmark</h2>

- **FEVER: A Large-Scale Dataset for Fact Extraction and Verification**. NAACL, 2018. [[paper](https://aclanthology.org/N18-1074/)]
- **FakeNewsNet: A Data Repository with News Content, Social Context, and Spatiotemporal Information for Studying Fake News on Social Media**. Big Data, 2020. [[paper](https://doi.org/10.1089/big.2020.0062)]
- **r/Fakeddit: A New Multimodal Benchmark Dataset for Fine-Grained Fake News Detection**. LREC, 2020. [[paper](https://aclanthology.org/2020.lrec-1.755/)]
- **PubHealthTab: A Public Health Table-Based Dataset for Evidence-Based Fact Checking**. Findings of NAACL, 2022. [[paper](https://aclanthology.org/2022.findings-naacl.1/)]
- **End-to-End Multimodal Fact-Checking and Explanation Generation: A Challenging Dataset and Models**. SIGIR, 2023. [[paper](https://doi.org/10.1145/3539618.3591879)]
- **FakeSV: A Multimodal Benchmark with Rich Social Context for Fake News Detection on Short Video Platforms**. AAAI, 2023. [[paper](https://doi.org/10.1609/aaai.v37i12.26689)]
- **RAGTruth: A Hallucination Corpus for Developing Trustworthy Retrieval-Augmented Language Models**. ACL, 2024. [[paper](https://aclanthology.org/2024.acl-long.585/)]
- **A New Dataset and Benchmark for Grounding Multimodal Misinformation**. ACM MM, 2025. [[paper](https://doi.org/10.1145/3746027.3758191)]
- **HalluLens: LLM Hallucination Benchmark**. ACL, 2025. [[paper](https://aclanthology.org/2025.acl-long.1176/)]
- **HalluMix: A Task-Agnostic, Multi-Domain Benchmark for Real-World Hallucination Detection**. arXiv, 2025. [[paper](https://arxiv.org/abs/2505.00506)]
- **MFC-Bench: Benchmarking Multimodal Fact-Checking with Large Vision-Language Models**. arXiv, 2025. [[paper](https://arxiv.org/abs/2406.11288)]
- **MMFakeBench: A Mixed-Source Multimodal Misinformation Detection Benchmark for LVLMs**. ICLR, 2025. [[paper](https://openreview.net/forum?id=YtY1jN3K0f)]
- **MMM-Fact: A Multimodal, Multi-Domain Fact-Checking Dataset with Multi-Level Retrieval Difficulty**. arXiv, 2025. [[paper](https://arxiv.org/abs/2510.25120)]
- **Worse than Zero-Shot? A Fact-Checking Dataset for Evaluating the Robustness of RAG Against Misleading Retrievals**. NeurIPS Datasets and Benchmarks, 2025. [[paper](https://proceedings.neurips.cc/paper_files/paper/2025/hash/ed25c00ff6900989116d3ba5d607d33d-Abstract-Datasets_and_Benchmarks_Track.html)]
- **XFacta: Contemporary, Real-World Dataset and Evaluation for Multimodal Misinformation Detection with Multimodal LLMs**. arXiv, 2025. [[paper](https://arxiv.org/abs/2508.09999)]
- **Drifting Away from Truth: GenAI-Driven News Diversity Challenges LVLM-Based Misinformation Detection**. AAAI, 2026. [[paper](https://doi.org/10.1609/aaai.v40i1.37023)]
- **FineFake: A Knowledge-Enriched Dataset for Fine-Grained Multi-Domain Fake News Detection**. Information Fusion, 2026. [[paper](https://doi.org/10.1016/j.inffus.2026.104253)]
- **Omni-Fake: Benchmarking Unified Multimodal Social Media Deepfake Detection**. CVPR, 2026. [[paper](https://openaccess.thecvf.com/content/CVPR2026/html/Li_Omni-Fake_Benchmarking_Unified_Multimodal_Social_Media_Deepfake_Detection_CVPR_2026_paper.html)]
- **The Coherence Trap: When MLLM-Crafted Narratives Exploit Manipulated Visual Contexts**. CVPR, 2026. [[paper](https://openaccess.thecvf.com/content/CVPR2026/html/Zhang_The_Coherence_Trap_When_MLLM-Crafted_Narratives_Exploit_Manipulated_Visual_Contexts_CVPR_2026_paper.html)]
- **The Synthetic Media Shift: Tracking the Rise, Virality, and Detectability of AI-Generated Multimodal Misinformation**. arXiv, 2026. [[paper](https://arxiv.org/abs/2604.15372)]
- **TriDF: Evaluating Perception, Detection, and Hallucination for Interpretable DeepFake Detection**. CVPR, 2026. [[paper](https://openaccess.thecvf.com/content/CVPR2026/html/Jiang-Lin_TriDF_Evaluating_Perception_Detection_and_Hallucination_for_Interpretable_DeepFake_Detection_CVPR_2026_paper.html)]
- **VLDBench: Evaluating Multimodal Disinformation with Regulatory Alignment**. Information Fusion, 2026. [[paper](https://doi.org/10.1016/j.inffus.2025.104092)]

---

<h2 id="future-direction">🚀 Future Direction</h2>

<h3 id="agentic-verification">Agentic Verification</h3>

Develop auditable verification agents that coordinate reasoning, retrieval, tools, and specialized models while preserving traceable evidence and intermediate decisions.

<h3 id="lifelong-detection">Lifelong Detection</h3>

Build continually evolving detectors that retain historical knowledge, adapt to emerging generators and misinformation patterns, and remain calibrated under temporal and domain shifts.

<h3 id="unified-system">Unified System</h3>

Unify content analysis, source assessment, evidence retrieval, propagation modeling, cross-modal consistency, and explanation within a shared veracity-centered system.

---

<h2 id="citation">✍️ Citation</h2>

The manuscript is currently under review and does not yet have a public preprint identifier. In the meantime, please use the following temporary citation; it will be replaced with the official bibliographic record once available.

```bibtex
@unpublished{dai2026misinformation,
  title={Misinformation Detection in the AIGC Era: Methods, Benchmarks, and Challenges},
  author={Dai, Juyi and Zeng, Yirong and Ding, Xiao and Luo, Jiashun and Cai, Bibo and You, Shen and Zang, Wenyu and Qin, Bing and Liu, Ting},
  note={Manuscript submitted to IEEE Transactions on Knowledge and Data Engineering},
  year={2026}
}
```

---

Maintained by the authors from Harbin Institute of Technology, SCIR.
