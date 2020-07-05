# CURL-pytorch-local-replay-buffer-assistance

This project is mainly a reimplementation of the CURL algorithm from this great [paper](https://arxiv.org/abs/1910.14481 "Continual Unsupervised Representation Learning") in pytorch. Their Tnsorflow source code is available at this [repo](https://github.com/deepmind/deepmind-research/tree/master/curl).

However, it is also an extension of their work where we investigated the used of a small replay buffer build using selective sampling based on un-similarity between samples. We have found that using such a replay buffer can help to prevent catastrophic forgetting, speacially when the selection is done at expansion time,  and that the contribution go beyond the simple use of a replay buffer. Additionnal details and results can be seen in the [project report](Project_report.pdf).

The notebook is splitted in 5 blocks:

- Imports: List of necesseary imports

- Dataloader: Construction of the dataset to be used.

- Models: Declaration of the pytorchs models.

- Functions: Declaration of the other functions.

- Experiment: Where the experiment is done and the list of hyperparameters are set.

