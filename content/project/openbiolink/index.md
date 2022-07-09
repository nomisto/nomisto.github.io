---
title: OpenBioLink
summary: A openly available large-scale biomedical knowledge graph.
tags:
- Knowledge Graph
- Biomedical Knowledge
- Link Prediction
date: "2019-12-01T00:00:00Z"

links:
- icon: github
  icon_pack: fab
  name: Code
  url: https://github.com/OpenBioLink/OpenBioLink
url_code: ""
url_pdf: "https://arxiv.org/abs/1912.04616"

---

OpenBioLink is a resource and evaluation framework for evaluating link prediction models on heterogeneous biomedical graph data. It contains benchmark datasets as well as tools for creating custom benchmarks and evaluating models.

The OpenBioLink benchmark aims to meet the following criteria:

- Openly available
- Large-scale
- Wide coverage of current biomedical knowledge and entity types
- Standardized, balanced train-test split
- Open-source code for benchmark dataset generation
- Open-source code for evaluation (independent of model)
- Integrating and differentiating multiple types of biological entities and relations (i.e., formalized as a heterogeneous graph)
- Minimized information leakage between train and test sets (e.g., avoid inclusion of trivially inferable relations in the test set)
- Coverage of true negative relations, where available
- Differentiating high-quality data from noisy, low-quality data
- Differentiating benchmarks for directed and undirected graphs in order to be applicable to a wide variety of link prediction methods
- Clearly defined release cycle with versions of the benchmark and public leaderboard

The OpenBioLink2020 Dataset is a highly challenging benchmark dataset containing over 5 million positive and negative edges. The test set does not contain trivially predictable, inverse edges from the training set and does contain all different edge types, to provide a more realistic edge prediction scenario.

## Datasets summary
|Dataset|Train|Test|Valid|Entities|Relations|
|-------|-----|----|-----|--------|---------|
|directed, high quality|8.503.580|401.901|397.066|184.732|28|
|undirected, high quality|7.559.921|372.877|357.297|184.722|28|
|directed, no quality cutoff|51.636.927|2.079.139|2.474.921|486.998|32|
|undirected, no quality cutoff|41.383.093|2.010.662|1.932.436|486.998|32|

## Baseline results    

| |       Model        |     MRR     |       h@1       |    h@10     |
|:-|:------------------|:-----------:|:---------------:|:-----------:|
||||||
|Latent|       RESCAL       |  **.320**   |      .212       |    .544     |
||       TransE       |    .280     |      .175       |    .500     |
||      DistMult      |    .300     |      .193       |    .521     |
||      ComplEx       |    .319     |      .211       |  **.547**   |
||       ConvE        |    .288     |      .186       |    .510     |
||       RotatE       |    .286     |      .180       |    .511     |
||||||
|Interpretable| AnyBURL (Maximum)  |    .277     |      .192       |    .457     |
|| AnyBURL (Noisy-OR) |    .159     |      .098       |    .295     |
||      SAFRAN\*      | <u>.306</u> | <u>**.214**</u> | <u>.501</u> |

Results are from [(LinkExplorer: Predicting, explaining and exploring links in large biomedical knowledge graphs; Ott et al)](https://www.biorxiv.org/content/10.1101/2022.01.09.475537v2). Embedding approaches were trained using [LibKGE](https://github.com/uma-pi1/kge). Best hyperparameters after extensive hyperparameter search can be found in the [supplementary material](https://www.biorxiv.org/content/biorxiv/early/2022/01/31/2022.01.09.475537/DC1/embed/media-1.pdf?download=true) of the before mentioned paper.

