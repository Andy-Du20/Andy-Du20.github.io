---
title: "SimPro: A Simple Probabilistic Framework Towards Realistic Long-Tailed Semi-Supervised Learning"
name: "SimPro"
authors: "**Chaoqun Du`*`**, Yizeng Han**`*`**, Gao Huang"
collection: publications
permalink: /publication/2024-05-01-paper-SimPro
excerpt: ""
date: 2024-05-01
venue: "ICML"
paperurl: "https://arxiv.org/pdf/2402.13505"
codeurl: "https://github.com/LeapLabTHU/SimPro"
#slidesurl: ""
#slidesurl: ""
#citation: ""
---

Recent advancements in semi-supervised learning
have focused on a more realistic yet challenging task: addressing imbalances in labeled data
while the class distribution of unlabeled data remains both unknown and potentially mismatched.
Current approaches in this sphere often presuppose rigid assumptions regarding the class distribution of unlabeled data, thereby limiting the
adaptability of models to only certain distribution ranges. In this study, we propose a novel
approach, introducing a highly adaptable framework, designated as SimPro, which does not rely
on any predefined assumptions about the distribution of unlabeled data. Our framework, grounded
in a probabilistic model, innovatively refines the
expectation-maximization (EM) algorithm by explicitly decoupling the modeling of conditional
and marginal class distributions. This separation
facilitates a closed-form solution for class distribution estimation during the maximization phase,
leading to the formulation of a Bayes classifier.
The Bayes classifier, in turn, enhances the quality
of pseudo-labels in the expectation phase. Remarkably, the SimPro framework not only comes
with theoretical guarantees but also is straightforward to implement. Moreover, we introduce two
novel class distributions broadening the scope of
the evaluation. Our method showcases consistent state-of-the-art performance across diverse
benchmarks and data distribution scenarios.

[Paper](https://arxiv.org/pdf/2402.13505) | [Code](https://github.com/LeapLabTHU/SimPro)
