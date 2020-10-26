# MMSR
# Matrix Mean-Subsequence-Reduced Algorithm
This repository contains code for our NeurIPS 2020 paper: [Adversarial Crowdsourcing Through Robust Rank-One Matrix Completion](https://arxiv.org/abs/2010.12181).


## Introduction
We consider the problem of reconstructing a rank-one matrix from a revealed subsetof its entries when some of the revealed entries are corrupted with perturbations thatare unknown and can be arbitrarily large. It is not known which revealed entries arecorrupted. We propose a new algorithm combining alternating minimization withextreme-value filtering and provide sufficient and necessary conditions to recoverthe original rank-one matrix. In particular, we show that our proposed algorithm isoptimal when the set of revealed entries is given by an Erdős-Rényi random graph.

These results are then applied to the problem of classification from crowdsourceddata under the assumption that while the majority of the workers are governed bythe standard single-coin David-Skene model (i.e., they output the correct answerwith a certain probability), some of the workers can deviate arbitrarily from thismodel. In particular, the “adversarial” workers could even make decisions designedto make the algorithm output an incorrect answer. Extensive experimental resultsshow our algorithm for this problem, based on rank-one matrix completion withperturbations, outperforms all other state-of-the-art methods in such an adversarialscenario.

## Code & datasets
### Datasets
The real datasets we used in our experiments are provided in this repository. They are dataset Fashion(Fashion1, Fashion2), TREC, Waterbird Datase (Bird), Dog, Temporal Ordering (Temp), Recognizing Textual Entailment(RTE), Web Search Relevance Judging (Web), Word Sense Disambiguation (WSD), Emotions (Fear, Surprise, Sadness, Disgust, Joy, Anger, Valence). The original datasets we are using are contained in the folder ./original_datasets. Since we consider crowdsourcing issues in adversarial setting in this work, we introduce adversaries for each dataset. The corrupted datasets with adversaries are contained in folder ./corrupted_datasets. The corrupted datasets can also be generated by using the files in folder ./corrupted_data_generation.

### Running the code
We provide the code of M-MSR, M-MSR-twocoin, as well as the code for baseline methods MV, KOS, GhostSVD, EoR, MV-D&S, PGD, OPT-D&S in the file ./MainProgram. The code for baseline methods BF-twocoin, MFA-twocoin, and EM-twocoin can be found at [website](https://www.cs.utexas.edu/~lqiang/publication.html), and the code for baseline methods Minmax, Entropy(O) can be found at [website](https://dennyzhou.github.io/).

## Authors
Welcome to send us Emails if you have any questions about the code and our work :-)
* **Qianqian Ma** (maqq@bu.edu)
* **Alex Olshevsky** [Website](http://sites.bu.edu/aolshevsky/)

## Citation
Please cite our paper if you like or use our work for your research, thank you very much!
