# Awesome Weight-Space Programming [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of work on **weight-space programming (WSP)**: language models that read, write or edit the weights of neural networks directly, without gradient descent, and of the earlier lines of work it builds on (programs compiled into weights, hypernetworks and text-to-weights models, LLM-written classical models, classifier weights from language, and gradient-free model editing).

The list has 145 entries. Every entry was checked against a primary page (arXiv record or full text, publisher or proceedings page, project page, or repository README) in November 2026. Most WSP items are blog posts, repositories or preprints that are not peer-reviewed; the venue column says so.

## Contents

- [Weight-space programming](#weight-space-programming)
  - [Core: the WSP post, its replications and the works it lists](#core-the-wsp-post-its-replications-and-the-works-it-lists)
  - [Follow-up papers (arXiv)](#follow-up-papers-arxiv)
  - [Critiques, controls and replications (outside arXiv)](#critiques-controls-and-replications-outside-arxiv)
  - [Applications: recognition, robustness and missing data](#applications-recognition-robustness-and-missing-data)
- [Predecessors](#predecessors)
  - [Programs compiled or written by hand into weights](#programs-compiled-or-written-by-hand-into-weights)
  - [Fast weight programmers, hypernetworks, text-to-weights and generative models of weights](#fast-weight-programmers-hypernetworks-text-to-weights-and-generative-models-of-weights)
  - [LLMs writing parameters of classical models from knowledge](#llms-writing-parameters-of-classical-models-from-knowledge)
  - [Classifier weights from language or in closed form for unseen classes](#classifier-weights-from-language-or-in-closed-form-for-unseen-classes)
  - [Gradient-free model editing guided by interpretability](#gradient-free-model-editing-guided-by-interpretability)
- [Contributing](#contributing)

## Weight-space programming

### Core: the WSP post, its replications and the works it lists

| Work | Venue / type, date | Links |
|---|---|---|
| Takehi, Teoh, Zhang, Khattab (MIT CSAIL), "Sparks of Weight-Space Programming: LLMs can natively read & write neural network weights" | Blog post, 2026-11-02; "Response to Comments" added 2026-11-12; not peer-reviewed | [Page](https://rikiyat.github.io/blog/weight-space-programming/) · [Code](https://github.com/RikiyaT/lm_understand-logs) |
| Hugging Face demo and model card (rebuild by Ahsen Khaliq; model repo by the first author) | HF Space and model card, Nov 2026 | [Hugging Face](https://huggingface.co/spaces/akhaliq/weight-space-programming-demo) · [Hugging Face](https://huggingface.co/RikiyaT/Qwen3.5-0.8B-weight-space-programming) |
| Simon Willison, "Qwen 3.8 27B on my laptop can interpret model weights, too" | Blog, 2026-11-03 | [Page](https://simonwillison.net/2026/Nov/3/qwen-can-interpret-model-weights/) |
| Matin Khajavi, "Weight-Space Programming Replication" | GitHub repository, Nov 2026 | [Code](https://github.com/MatinKhajavi/Weight-Space-Programming) |
| statsleelab, "Sparks of Weight-Space Programming: Complete Reproduction & Interactive Guide" | GitHub repository, Nov 2026 | [Code](https://github.com/statsleelab/weight_space_programming) |
| Gong, Zheng, Huang, Chen, Tian, Yang, Liu, Yang (Shanghai Innovation Institute, SJTU, HKU), "We Asked Opus-5.5 to Edit pi0.5's Weights. AutoResearch Made It Happen." | Project page, Nov 2026 | [Page](https://cuzyoung.github.io/robotics-weight-editing/en/) |
| Kundu, Ghosh, Honavar (Penn State), "Weight-Space Programming of Variational Quantum Circuits: Large Language Models Write Quantum Circuit Parameters Without an Optimizer" | arXiv 2611.11537, 2026-11-08, preprint | [Paper](https://arxiv.org/abs/2611.11537) |
| Chandan Singh, "Weight-space programming from scratch on simple tasks"; then Mehta, Singh, Xu, Antonello, Flinker, Mesgarani, Bonner, Jojic, Gao (Microsoft Research, Johns Hopkins, Columbia, NYU), "Interpretable weight-space programming builds transparent transformers and brain encoding models" (iWSP) | Report 2026-11-02; arXiv 2611.18114v1, 2026-11-13, preprint, 33 pages | [Page](https://csinva.io/weight-space-programming-autoresearch/analyze/toy_examples/report.html) · [Paper](https://arxiv.org/abs/2611.18114) · [Code](https://github.com/csinva/weight-space-programming-autoresearch) |
| von Csefalvay, Doma, Krishnan, Földi (HCLTech), "IWIBench: Evaluating Gradient-Free Model Driven Intra-weight Injection" | arXiv 2611.08647, 2026-11-05, preprint | [Paper](https://arxiv.org/abs/2611.08647) |
| Lindholz et al. (Charité and others), "Weight-Space Programming for Medical Imaging: Do We Still Need Training Data?" | arXiv 2611.12066, 2026-11-09, preprint | [Paper](https://arxiv.org/abs/2611.12066) |
| Nusrat and Nusrat (Henry Ford Health; Toronto Metropolitan University), "Weight-space programming for auditing clinical decision networks" | arXiv 2611.05341, 2026-11-03, preprint | [Paper](https://arxiv.org/abs/2611.05341) |
| Varam, Najafi, Atienza (EPFL), "Mixed Signals: Weight-Space Programming for EEG and ECG" | arXiv 2611.13758, 2026-11-10, preprint | [Paper](https://arxiv.org/abs/2611.13758) |
| Bruni Cardoso, "Weight-space programming on a regulatory-genomics CNN: public release 1" | GitHub repository with preprint and Zenodo DOI 10.5281/zenodo.24040591; preregistered; Nov 2026 | [Code](https://github.com/brunicardoso/weight-space-programming-genomics) |
| Manas Karra, "Piano to flute, one weight edit" | Blog, 2026-11-08 | [Page](https://manaskarra.com/blog/magenta-wsp) |
| AdderBoard (maintained by Dimitris Papailiopoulos); cited by the post as prior work | GitHub leaderboard | [Code](https://github.com/anadim/AdderBoard) |

### Follow-up papers (arXiv)

| Work | Venue / type, date | Links |
|---|---|---|
| Goworek, Hickey, Nanni, O'Reilly (The Alan Turing Institute), "Replicating and Extending Weight-Space Programming: Frontier LLMs Compile Programs into Weights and Read Input Layers" | arXiv 2611.21449, 2026-11-16 | [Paper](https://arxiv.org/abs/2611.21449) |
| Subham Kundu (TCG Crest), "Same Fix, Different Weights: Replicating Weight-Space Programming with Claude" | arXiv 2611.20953, 2026-11-16 | [Paper](https://arxiv.org/abs/2611.20953) |
| Matteo Fischetti, "Just sort it! A note on the LP behind rank-one anti-loop edits" | arXiv 2611.21432, 2026-11-16 | [Paper](https://arxiv.org/abs/2611.21432) |
| Salloum and Ali, "Tree-Ising: Repairing Language Models with Bit-Level Ising Edits" | arXiv 2611.14210, 2026-11-10 | [Paper](https://arxiv.org/abs/2611.14210) |
| Nazmus Sakib Ahmed, "Can an LLM Actually Reason and Program about Neural Network's Weights or is it just memorization on steroids? Exploring 'Weight-Space Programming'" | arXiv 2611.08070, 2026-11-05 | [Paper](https://arxiv.org/abs/2611.08070) |
| Liu and Yang, "Computation, not weight access: large language models as auditors of clinical prediction networks" | arXiv 2611.07847, 2026-11-05 (v2 2026-11-06) | [Paper](https://arxiv.org/abs/2611.07847) |
| Hu, Tang, Li, Zhu, Feng, Zhang, Chen, Hu, "Exploring Weight-Space Programming: Capabilities, Generalization, and Limitations" | arXiv 2611.09382, 2026-11-06 | [Paper](https://arxiv.org/abs/2611.09382) |
| Marasini, Khadka, Rahimi, "WeightBench: Evaluating Language Models as Weight-Space Programmers" | arXiv 2611.18553, 2026-11-13 | [Paper](https://arxiv.org/abs/2611.18553) |
| Jens Lehmann, "Compiling Known Rules into Compact Neural Agents: Weight-Space Programming on Unseen Games" | arXiv 2611.16981, 2026-11-12 | [Paper](https://arxiv.org/abs/2611.16981) |
| Eduardo C. Garrido-Merchán, "Zero-Shot Weight-Space Programming Across a Difficulty-Graded Ladder of Two-Player Games" | arXiv 2611.09271, 2026-11-06 (v2 2026-11-09) | [Paper](https://arxiv.org/abs/2611.09271) |
| Eduardo C. Garrido-Merchán, "Zero-Shot Weight-Space Programming for Prediction and Classification of Target Variables in Structured Datasets" | arXiv 2611.19292, 2026-11-14 | [Paper](https://arxiv.org/abs/2611.19292) |
| Hoo, Buehler, Swelam, Hutter, Purucker, "Weights & Caches: LLMs Can Program Tabular Foundation Models" | arXiv 2611.20174, 2026-11-15 | [Paper](https://arxiv.org/abs/2611.20174) |
| Dennis Gross, "Weight-Space Programming of Policies and Their Verification via Model Checking" | arXiv 2611.11604, 2026-11-08 | [Paper](https://arxiv.org/abs/2611.11604) |
| Sato, Shimada, Murasaki, Sano, "Physics2Weight: Direct Neural Network Architecture and Weight Generation from Physical Laws Using Large Language Models" | arXiv 2611.12954, 2026-11-07 | [Paper](https://arxiv.org/abs/2611.12954) |
| Renan Butkeraites, "Can a Language Model Write the Weights? An Empirical Study of LLM-Written Scoring Networks for Column Generation and MILP Branching, with a Bus-Driver Scheduling Application" | arXiv 2611.09559, 2026-11-06 | [Paper](https://arxiv.org/abs/2611.09559) |
| Zhang, Wang, Lin, "Can LLMs Debug Robots by Editing Their Weights?" | arXiv 2611.09376, 2026-11-06 | [Paper](https://arxiv.org/abs/2611.09376) |
| Abbas and Seraj, "Distilling Instructions into Weights: Closed-Form Edits Fix a Robot Policy's Misreading" | arXiv 2611.11894, 2026-11-09 | [Paper](https://arxiv.org/abs/2611.11894) |
| Wang, Lu, Li, "Can LLMs Write Backdoors? An Empirical Security Study of Weight-Space Programming" | arXiv 2611.17395, 2026-11-12 | [Paper](https://arxiv.org/abs/2611.17395) |
| Li, Li, Zhao, Zhang, Zhang, Xu, Zang, Leung, Li, "WeightLoop: Weight-Space Programming with Experimental Feedback" | arXiv 2611.07319, 2026-11-05 (v2 2026-11-14) | [Paper](https://arxiv.org/abs/2611.07319) |
| Makoto Sato, "Weight-Space Programming Changes How an LLM Uses Python for Computational Biology" | arXiv 2611.20566, 2026-11-16 | [Paper](https://arxiv.org/abs/2611.20566) |
| Mohamed Abdallah Salem, "Can Large Language Models Optimize Pretrained Neural Network Weights? A Multi-Phase Empirical Evaluation of Gradient-Free Editing in YOLO26 Object Detection" | arXiv 2611.17789, 2026-11-13 | [Paper](https://arxiv.org/abs/2611.17789) |
| Zheng and Zheng, "Perceptual Weight Space Programming for Diffusion Super-Resolution" | arXiv 2611.18690, 2026-11-03 | [Paper](https://arxiv.org/abs/2611.18690) |
| Zheng and Doubao, "Weight-Space Programming for Improving Image-Restoration Diffusion Models: Technical Conjectures and a Recursive Improvement Loop" | arXiv 2611.04268, 2026-11-03 | [Paper](https://arxiv.org/abs/2611.04268) |
| Fu, Zhao, Korakakis, Ding, Szpruch, Zhang, "SWEET: Mitigating Spurious Feature Reliance in LLM Reasoning via Weight Editing" | arXiv 2611.10974, 2026-11-07 | [Paper](https://arxiv.org/abs/2611.10974) |

### Critiques, controls and replications (outside arXiv)

| Work | Venue / type, date | Links |
|---|---|---|
| Matthew Honnibal, "The 'Astra can read and write weights to improve Qwen' post is misleading" | Blog, 2026-11-03 | [Page](https://honnibal.dev/blog/astra-read-write-misleading) |
| Sean Goedecke, "LLMs are not superhuman at reading and writing neural network weights" | Blog, 2026-11-03 | [Page](https://www.seangoedecke.com/llms-are-not-superhuman-at-reading-and-writing-neural-network-weights/) |
| Andreas Maier, "Weight-Space Programming: What Is Measured and What Is Anecdote" | Substack, 2026-11-05 | [Page](https://akmaier.substack.com/p/weight-space-programming-what-is) |
| Yiqun Zhang, "Rethinking Weight-Space Programming: Re-running the experiments with baselines and controls" | GitHub repository and blog, Nov 2026 | [Code](https://github.com/ZhangYiqun018/rethinking-weight-space-programming) |
| Zhang, Shang, Li (UBC, Vector Institute), "EditLens: What Did Astra's Edit Actually Do?" | Research essay, Nov 2026 | [Page](https://xxlya.github.io/editlens/) |
| Khamis, Tutunov, Bou Ammar, "Who Needs an LLM to Program an LLM? Introducing AHA!" | Web article, 2026-11-15 | [Page](https://haithamb.github.io/aha/) |
| goddoe, "Weight-Space Programming: an independent reproduction" | GitHub repository, Nov 2026 | [Code](https://github.com/goddoe/weight-space-programming) |
| hamley241, "weight-space-horizon" | GitHub repository, preregistered, Nov 2026 | [Code](https://github.com/hamley241/weight-space-horizon) |
| hamley241, "Can a language model repair a network's weights by reading them?" | GitHub repository with an extended abstract (workshop style), 2026-11-07 | [Code](https://github.com/hamley241/wsp-harness-public) |
| dhaneshnm, "Does Claude have it too? A replication of Weight-Space Programming" | GitHub repository, 2026-11-06 | [Code](https://github.com/dhaneshnm/wsp-replication) |
| MaceTenth, "Can an AI read and edit another AI's weights? We tested the MIT CSAIL claim with Claude" | GitHub repository, Nov 2026 | [Code](https://github.com/MaceTenth/weight-space-programming-replication) |
| Sabhya Chhabria, "[WIP] Can Opus 5.5 teach an image model what 'no' means?" | Blog, 2026-11-02, marked work in progress | [Page](https://sabhyachhabria.com/writing/weight-space-negation/) |
| Ok and Lee (POSTECH), "Weight-Space Programming Doesn't Need Transformers" | GitHub repository and project page, Nov 2026 | [Code](https://github.com/effl-lab/Weight-Space-Programming) |
| SajjadPSavoji, "Awesome Weight-Space Programming" | Curated list, updated daily | [Code](https://github.com/SajjadPSavoji/awesome-weight-space-programming) |

### Applications: recognition, robustness and missing data

| Work | Venue / type, date | Links |
|---|---|---|
| Javier Solís-García (first author of CoSTI) with an agent ("Astra 6 Max" in OpenAI Codex), "Weight-space programming on CoSTI" | GitHub repository; session of 2026-11-03 | [Code](https://github.com/javiersgjavi/costi-weight-space-programming) |
| waliddev23, "Weight-space programming on EuroSAT" | GitHub repository, Nov 2026 | [Code](https://github.com/waliddev23/weight_space_programming_for_remote_sensing_a_small_case_study) |
| SuyodhanJ6, "Weight-Space Programming (WSP)" (cats vs dogs) | GitHub repository, Nov 2026 | [Code](https://github.com/SuyodhanJ6/weight-space-programming) |
| apetcu, "Weight-space programming on a character recognizer" | GitHub repository, 2026-11-07 | [Code](https://github.com/apetcu/weight-space-programming) |
| canyon-tractian, "Teaching a detector a new object by writing its weights by hand" (wsp-detect) | GitHub repository, Nov 2026 | [Code](https://github.com/canyon-tractian/wsp-detect) |
| sfc-gh-tosmith, "Banking77 by weight-space programming" | GitHub repository, Nov 2026 | [Code](https://github.com/sfc-gh-tosmith/wsp-banking77) |
| KristinaMruts, "Weight-space programming on a clinical splicing model" | GitHub repository, Nov 2026 | [Code](https://github.com/KristinaMruts/weight-space-programming-spliceai) |
| mrtpk, "wsp-yolo-eel" | GitHub repository, Nov 2026 | [Code](https://github.com/mrtpk/wsp-yolo-eel) |

## Predecessors

### Programs compiled or written by hand into weights

| Work | Venue / type, date | Links |
|---|---|---|
| Weiss, Goldberg, Yahav, "Thinking Like Transformers" (RASP) | ICML 2021 (arXiv comment) | [Paper](https://arxiv.org/abs/2106.06981) |
| Lindner, Kramár, Farquhar, Rahtz, McGrath, Mikulik, "Tracr: Compiled Transformers as a Laboratory for Interpretability" (cited by the post) | NeurIPS 2023 spotlight (arXiv comment) | [Paper](https://arxiv.org/abs/2301.05062) |
| Shaw, Cohan, Eisenstein, Lee, Berant, Toutanova, "ALTA: Compiler-Based Analysis of Transformers" | TMLR 2025 (arXiv comment) | [Paper](https://arxiv.org/abs/2410.18077) |
| Friedman, Wettig, Chen, "Learning Transformer Programs" | NeurIPS 2023 oral (arXiv comment) | [Paper](https://arxiv.org/abs/2306.01128) |
| Giannou, Rajput, Sohn, Lee, Lee, Papailiopoulos, "Looped Transformers as Programmable Computers" | arXiv, 2023-01 | [Paper](https://arxiv.org/abs/2301.13196) |
| Thurnherr and Scheurer, "TracrBench: Generating Interpretability Testbeds with Large Language Models" | ICML Mechanistic Interpretability Workshop (arXiv comment), 2024-09 | [Paper](https://arxiv.org/abs/2409.13714) |
| Vergara-Browne and Soto, "Tracr-Injection: Distilling Algorithms into Pre-trained Language Models" | ACL Findings 2025 (arXiv comment) | [Paper](https://arxiv.org/abs/2505.10719) |
| Weber, Michel, Renda, Carbin, "Learning to Compile Programs to Neural Networks" | arXiv, 2024-07 | [Paper](https://arxiv.org/abs/2407.15078) |
| Zhang, Hotsko, Kim, Nie, Shieber, Deng, "Program-as-Weights: A Programming Paradigm for Fuzzy Functions" | NeurIPS 2026 | [Paper](https://arxiv.org/abs/2607.02512) · [Demo](https://programasweights.com/playground) |
| Bunel, Desmaison, Kohli, Torr, Kumar, "Adaptive Neural Compilation" | arXiv, 2016-05 | [Paper](https://arxiv.org/abs/1605.07969) |
| Gruau, Ratajszczak, Wiber, "A neural compiler" | Theoretical Computer Science 141, 1995 | [DOI](https://doi.org/10.1016/0304-3975(94) |
| Towell and Shavlik, "Knowledge-based artificial neural networks" (KBANN) | Artificial Intelligence 70, 1994 | [DOI](https://doi.org/10.1016/0004-3702(94) |
| Akyürek, Schuurmans, Andreas, Ma, Zhou, "What learning algorithm is in-context learning? Investigations with linear models"; von Oswald et al., "Transformers learn in-context by gradient descent" | ICLR 2023 (arXiv comment); arXiv 2022-12 | [Paper](https://arxiv.org/abs/2211.15661) · [Paper](https://arxiv.org/abs/2212.07677) |
| Theia Vogel, "I made a transformer by hand (no training!)" | Blog, 2023-09-11 | [Page](https://vgel.me/posts/handmade-transformer/) |

### Fast weight programmers, hypernetworks, text-to-weights and generative models of weights

| Work | Venue / type, date | Links |
|---|---|---|
| Schmidhuber, "Learning to Control Fast-Weight Memories: An Alternative to Dynamic Recurrent Networks" | Neural Computation 4(1), 1992 | [DOI](https://doi.org/10.1162/neco.1992.4.1.131) |
| Schlag, Irie, Schmidhuber, "Linear Transformers Are Secretly Fast Weight Programmers" (the arXiv 2102.11174 cited by the post) | ICML 2021 (OpenAlex) | [Paper](https://arxiv.org/abs/2102.11174) |
| Ha, Dai, Le, "HyperNetworks" | arXiv, 2016-09 | [Paper](https://arxiv.org/abs/1609.09106) |
| Knyazev, Drozdzal, Taylor, Romero-Soriano, "Parameter Prediction for Unseen Deep Architectures" (GHN-2) | NeurIPS 2021 (arXiv comment) | [Paper](https://arxiv.org/abs/2110.13100) |
| Knyazev, Hwang, Lacoste-Julien, "Can We Scale Transformers to Predict Parameters of Diverse ImageNet Models?" | ICML 2023 (arXiv comment) | [Paper](https://arxiv.org/abs/2303.04143) |
| Peebles, Radosavovic, Brooks, Efros, Malik, "Learning to Learn with Generative Models of Neural Network Checkpoints" (G.pt) | arXiv, 2022-09 | [Paper](https://arxiv.org/abs/2209.12892) |
| Wang et al., "Neural Network Diffusion" (p-diff) | arXiv, 2024-02 | [Paper](https://arxiv.org/abs/2402.13144) |
| Wang, Tang, Zhao, Schürholt, Wang, You, "Recurrent Diffusion for Large-Scale Parameter Generation" (RPG) | arXiv, 2025-01 | [Paper](https://arxiv.org/abs/2501.11587) |
| Gupta, Biggs, Laber, Shafi, Walters, Paul, "DeepWeightFlow: Re-Basined Flow Matching for Generating Neural Network Weights" | ICLR 2026 (arXiv journal reference) | [Paper](https://arxiv.org/abs/2601.05052) |
| Biggs, Soro, Gupta, Andreis, Hwang, "A Night at the LLM Zoo: Data Conditioned Flow Matching for Generating Pretrained LLM Weights" | arXiv 2611.07103, 2026-11-04 | [Paper](https://arxiv.org/abs/2611.07103) |
| Zeng, Yin, Xu, Liu, "Generative Modeling of Weights: Generalization or Memorization?" | arXiv, 2025-06 | [Paper](https://arxiv.org/abs/2506.07998) |
| Ye and Ren, "Learning to Generate Task-Specific Adapters from Task Description" (Hypter) | ACL 2021 (arXiv comment) | [Paper](https://arxiv.org/abs/2101.00420) |
| Phang, Mao, He, Chen, "HyperTuning: Toward Adapting Large Language Models without Back-propagation" | arXiv, 2022-11 | [Paper](https://arxiv.org/abs/2211.12485) |
| Charakorn, Cetin, Tang, Lange, "Text-to-LoRA: Instant Transformer Adaption" | ICML 2025 (arXiv comment) | [Paper](https://arxiv.org/abs/2506.06105) |
| Liang et al., "Drag-and-Drop LLMs: Zero-Shot Prompt-to-Weights" | arXiv, 2025-06 | [Paper](https://arxiv.org/abs/2506.16406) |
| Charakorn, Cetin, Uesaka, Lange, "Doc-to-LoRA: Learning to Instantly Internalize Contexts" | arXiv 2602.15902, 2026-02 | [Paper](https://arxiv.org/abs/2602.15902) |
| Cheng, Shi, Zhang, Li, "The Override Gap: A Magnitude Account of Knowledge Conflict Failure in Hypernetwork-Based Instant LLM Adaptation" | arXiv 2604.23750, 2026-04 | [Paper](https://arxiv.org/abs/2604.23750) |
| Wang, Zhang, Li, "NeuronGen: Neural Network Parameter Generation via Large Language Models" | arXiv 2505.12470, 2025-05 (v3 2026-11) | [Paper](https://arxiv.org/abs/2505.12470) |
| Bianchi et al., "Robotic Policy Adaptation via Weight-Space Meta-Learning" (WIZARD) | arXiv 2606.07217, 2026-06 | [Paper](https://arxiv.org/abs/2606.07217) |
| Ruiz et al., "HyperDreamBooth: HyperNetworks for Fast Personalization of Text-to-Image Models" | arXiv, 2023-07 | [Paper](https://arxiv.org/abs/2307.06949) |
| Wang, Wang, Wang, "Position: Weight Space Should Be a First-Class Generative AI Modality" | arXiv 2605.18632, 2026-05 | [Paper](https://arxiv.org/abs/2605.18632) |
| Kabra, Venhoff, Schroeder de Witt, "Weight Oracles: Reading Neural Network Weights with Language Models" | arXiv 2610.07334, 2026-10; spotlight at a NeurIPS 2026 workshop (arXiv comment) | [Paper](https://arxiv.org/abs/2610.07334) |

### LLMs writing parameters of classical models from knowledge

| Work | Venue / type, date | Links |
|---|---|---|
| Jeong, Lipton, Ravikumar, "LLM-Select: Feature Selection with Large Language Models" | TMLR, April 2025 (arXiv comment) | [Paper](https://arxiv.org/abs/2407.02694) |
| Zhang et al., "LLM-Lasso: A Robust Framework for Domain-Informed Feature Selection and Regularization" | arXiv, 2025-02 | [Paper](https://arxiv.org/abs/2502.10648) |
| Capstick, Krishnan, Barnaghi, "AutoElicit: Using Large Language Models for Expert Prior Elicitation in Predictive Modelling" | arXiv, 2024-11 | [Paper](https://arxiv.org/abs/2411.17284) |
| Selby et al., "Had enough of experts? Quantitative knowledge retrieval from large language models" | Stat 14, 2025 (arXiv journal reference) | [Paper](https://arxiv.org/abs/2402.07770) |
| Riegler, Hellton, Thambawita, Hammer, "Using Large Language Models to Suggest Informative Prior Distributions in Bayesian Statistics" | arXiv, 2025-06 | [Paper](https://arxiv.org/abs/2506.21964) |
| Knauer et al., "'Oh LLM, I'm Asking Thee, Please Give Me a Decision Tree': Zero-Shot Decision Tree Induction and Embedding with Large Language Models" | KDD 2025 Research Track (arXiv comment) | [Paper](https://arxiv.org/abs/2409.18594) |
| Carrasco, Urrutia, Abeliuk, "Zero-Shot Decision Tree Construction via Large Language Models" | arXiv, 2025-01 | [Paper](https://arxiv.org/abs/2501.16247) |
| Han, Yoon, Arik, Pfister, "Large Language Models Can Automatically Engineer Features for Few-Shot Tabular Learning" (FeatLLM) | ICML 2024 (arXiv comment) | [Paper](https://arxiv.org/abs/2404.09491) |
| Yang et al., "Large Language Models as Optimizers" (OPRO) | ICLR 2024 (arXiv comment) | [Paper](https://arxiv.org/abs/2309.03409) |
| Lange, Tian, Tang, "Large Language Models As Evolution Strategies" | arXiv, 2024-02 | [Paper](https://arxiv.org/abs/2402.18381) |

### Classifier weights from language or in closed form for unseen classes

| Work | Venue / type, date | Links |
|---|---|---|
| Elhoseiny, Saleh, Elgammal, "Write a Classifier: Zero-Shot Learning Using Purely Textual Descriptions" | ICCV 2013 (OpenAlex, DOI 10.1109/ICCV.2013.321) | [DOI](https://doi.org/10.1109/ICCV.2013.321) |
| Frome et al., "DeViSE: A Deep Visual-Semantic Embedding Model" | NeurIPS 2013 (OpenAlex) | [Page](http://papers.nips.cc/paper/5204-devise-a-deep-visual-semantic-embedding-model.pdf) |
| Ba, Swersky, Fidler, Salakhutdinov, "Predicting Deep Zero-Shot Convolutional Neural Networks using Textual Descriptions" | ICCV 2015 (arXiv comment) | [Paper](https://arxiv.org/abs/1506.00511) |
| Changpinyo, Chao, Gong, Sha, "Synthesized Classifiers for Zero-Shot Learning" | CVPR 2016 (OpenAlex, DOI 10.1109/CVPR.2016.575) | [Paper](https://arxiv.org/abs/1603.00550) |
| Wang, Ye, Gupta, "Zero-shot Recognition via Semantic Embeddings and Knowledge Graphs" | CVPR 2018 (arXiv comment) | [Paper](https://arxiv.org/abs/1803.08035) |
| Qi, Brown, Lowe, "Low-Shot Learning with Imprinted Weights" | CVPR 2018 (arXiv comment) | [Paper](https://arxiv.org/abs/1712.07136) |
| Gidaris and Komodakis, "Dynamic Few-Shot Visual Learning without Forgetting" | CVPR 2018 (arXiv comment) | [Paper](https://arxiv.org/abs/1804.09458) |
| Radford et al., "Learning Transferable Visual Models From Natural Language Supervision" (CLIP) | arXiv, 2021-02 | [Paper](https://arxiv.org/abs/2103.00020) |
| Menon and Vondrick, "Visual Classification via Description from Large Language Models" | arXiv, 2022-10 | [Paper](https://arxiv.org/abs/2210.07183) |
| Pratt, Covert, Liu, Farhadi, "What does a platypus look like? Generating customized prompts for zero-shot image classification" (CuPL) | ICCV 2023 (arXiv comment) | [Paper](https://arxiv.org/abs/2209.03320) |
| Roth, Kim, Koepke, Vinyals, Schmid, Akata, "Waffling around for Performance: Visual Classification with Random Words and Broad Concepts" (WaffleCLIP) | ICCV 2023 (arXiv comment) | [Paper](https://arxiv.org/abs/2306.07282) |
| Zhang et al., "Tip-Adapter: Training-Free Adaption of CLIP for Few-Shot Classification" | ECCV 2022 (Crossref, DOI 10.1007/978-3-031-19833-5_29) | [Paper](https://arxiv.org/abs/2111.03930) |
| Christensen, Mancini, Koepke, Winther, Akata, "Image-free Classifier Injection for Zero-Shot Classification" (ICIS) | ICCV 2023 (arXiv comment) | [Paper](https://arxiv.org/abs/2308.10599) |
| Amosy, Volk, Shapira, Ben-David, Reichart, Chechik, "Text2Model: Text-based Model Induction for Zero-shot Image Classification" | Findings of EMNLP 2024 (Crossref, DOI 10.18653/v1/2024.findings-emnlp.8) | [Paper](https://arxiv.org/abs/2210.15182) |
| Lyu, Wang, Ban, Chen, Zhou, Chen, "Expanding the Category of Classifiers with LLM Supervision" (CEMIL) | IJCAI 2025, pages 5905-5913 | [Paper](https://www.ijcai.org/proceedings/2025/657) |
| Heyden, Ullah, Siddiqui, Al Machot, "CAST: Closed-form Analytic Semantic Transfer for Zero-Shot Classifier Extension" | arXiv 2608.13751, 2026-08 | [Paper](https://arxiv.org/abs/2608.13751) |
| Xiang, Li, Zhou, Wang, Zhang, "Generative Action Description Prompts for Skeleton-based Action Recognition" (GAP) | ICCV 2023 (arXiv comment) | [Paper](https://arxiv.org/abs/2208.05318) |
| Zhu, Ke, Gong, Bailey, "Part-aware Unified Representation of Language and Skeleton for Zero-shot Action Recognition" (PURLS) | CVPR 2024 (OpenAlex, DOI 10.1109/CVPR52733.2024.01775) | [Paper](https://arxiv.org/abs/2406.13327) |
| Zhu, Zhu, Rahmani, Liu, Bennamoun, Ke, "Boosting Skeleton-based Zero-Shot Action Recognition with Training-Free Test-Time Adaptation" (Skeleton-Cache) | arXiv 2512.11458, 2025-12 | [Paper](https://arxiv.org/abs/2512.11458) |

### Gradient-free model editing guided by interpretability

| Work | Venue / type, date | Links |
|---|---|---|
| Bau, Liu, Wang, Zhu, Torralba, "Rewriting a Deep Generative Model" | ECCV 2020 oral (arXiv comment) | [Paper](https://arxiv.org/abs/2007.15646) |
| Santurkar, Tsipras, Elango, Bau, Torralba, Madry, "Editing a classifier by rewriting its prediction rules" | NeurIPS 2021 (OpenAlex) | [Paper](https://arxiv.org/abs/2112.01008) |
| Meng, Bau, Andonian, Belinkov, "Locating and Editing Factual Associations in GPT" (ROME) | NeurIPS 2022 (arXiv comment) | [Paper](https://arxiv.org/abs/2202.05262) |
| Meng, Sen Sharma, Andonian, Belinkov, Bau, "Mass-Editing Memory in a Transformer" (MEMIT) | arXiv, 2022-10 | [Paper](https://arxiv.org/abs/2210.07229) |
| Orgad, Kawar, Belinkov, "Editing Implicit Assumptions in Text-to-Image Diffusion Models" (TIME) | arXiv, 2023-03 | [Paper](https://arxiv.org/abs/2303.08084) |
| Gandikota, Orgad, Belinkov, Materzyńska, Bau, "Unified Concept Editing in Diffusion Models" | WACV 2024 (arXiv comment) | [Paper](https://arxiv.org/abs/2308.14761) |
| Ilharco et al., "Editing Models with Task Arithmetic" | ICLR 2023 (arXiv comment) | [Paper](https://arxiv.org/abs/2212.04089) |
| Belrose et al., "LEACE: Perfect linear concept erasure in closed form" | NeurIPS 2023 (OpenAlex) | [Paper](https://arxiv.org/abs/2306.03819) |
| Arditi et al., "Refusal in Language Models Is Mediated by a Single Direction" | NeurIPS 2024 (OpenAlex) | [Paper](https://arxiv.org/abs/2406.11717) |
| Gandelsman, Efros, Steinhardt, "Interpreting CLIP's Image Representation via Text-Based Decomposition" | arXiv, 2023-10 | [Paper](https://arxiv.org/abs/2310.05916) |
| Gandelsman, Efros, Steinhardt, "Interpreting the Second-Order Effects of Neurons in CLIP" | arXiv, 2024-06 | [Paper](https://arxiv.org/abs/2406.04341) |
| Chuang, Jampani, Li, Torralba, Jegelka, "Debiasing Vision-Language Models via Biased Prompts" | arXiv, 2023-01 | [Paper](https://arxiv.org/abs/2302.00070) |
| Adila, Shin, Cai, Sala, "Zero-Shot Robustification of Zero-Shot Models" (RoboShot) | ICLR 2024 (arXiv comment) | [Paper](https://arxiv.org/abs/2309.04344) |
| Shaham et al., "A Multimodal Automated Interpretability Agent" (MAIA) | arXiv, 2024-04 | [Paper](https://arxiv.org/abs/2404.14394) |
| Shah, Ilyas, Madry, "Decomposing and Editing Predictions by Modeling Model Computation" (COAR) | arXiv, 2024-04 | [Paper](https://arxiv.org/abs/2404.11534) |
| Yang, Huang, Chen, Ma, Wei, "Learning Where to Edit Vision Transformers" | arXiv, 2024-11 | [Paper](https://arxiv.org/abs/2411.01948) |
| Kirichenko, Izmailov, Wilson, "Last Layer Re-Training is Sufficient for Robustness to Spurious Correlations" | ICLR 2023 (arXiv comment) | [Paper](https://arxiv.org/abs/2204.02937) |
| Li, Wang, Shi, Liu, Hou, "Revisiting Batch Normalization For Practical Domain Adaptation" (AdaBN) | arXiv, 2016-03 | [Paper](https://arxiv.org/abs/1603.04779) |
| Iwasawa and Matsuo, "Test-Time Classifier Adjustment Module for Model-Agnostic Domain Generalization" (T3A) | NeurIPS 2021 | [Paper](https://proceedings.neurips.cc/paper_files/paper/2021/hash/1415fe9fea0fa1e45dddcff5682239a0-Abstract.html) |

## Contributing

Pull requests are welcome. Please add one row per work with the title, authors, venue (or "arXiv preprint", "blog post", "repository") and date, and links to the paper and code. Add a work only after opening its primary page; do not add entries from memory or from secondary write-ups.

## License

[CC0 1.0](LICENSE)
