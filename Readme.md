# DeMinify: Neural Variable Name Recovery and Type Inference for Minified Code

<p aligh="center"> This repository contains the code for <b>DeMinify: Neural Variable Name Recovery and Type Inference for Minified Code</b>.</p>

# Source Code: https://github.com/variable-name-type-prediction/variable-name-type-prediction#Instruction_to_Run_DeMinify


## Contents
1. [Introduction](#Introduction)
2. [Dataset](#Dataset)
3. [Requirement](#Requirement)
4. [Instruction_to_Run_DeMinify](#Instruction_to_Run_DeMinify)

## Introduction

To avoid the exposure of original source code, the variable names deployed in the wild are often replaced by short, meaningless names,
thus making the code difficult to understand and be analyzed. We
introduce DeMinify, a Deep-Learning (DL)-based approach that
formulates such recovery problem as the predicting the missing features in the Graph Convolutional Network–Missing Features. The
graph represents both the relations among the variables and those
among their types, in which names/types of some nodes are missing.
Moreover, DeMinify leverages dual-task learning to propagate the
mutual impact between the learning of the variable names and that
of their types. We conducted experiments to evaluate DeMinify in
both name recovery and type prediction on a real-world dataset
with 180k Python methods. For variable name prediction, in 76.7%
of the cases, DeMinify can predict correctly the variables’ names
with a single suggested name. DeMinify relatively improves from
15.3–40.7% in top-1 accuracy over the state-of-the-art variable name
recovery approaches. It relatively improves 14.5%–51.9% in top-1
accuracy over the existing type prediction approaches. We showed
that learning of types help improve variable name recovery.


## Dataset

We use the dataset from existing benchmark python dataset: [ManyTypes4Py: A Benchmark Python Dataset for Machine Learning-based Type Inference](https://github.com/saltudelft/many-types-4-py-dataset)

## Requirement

Install ```Torch``` by following the Instruction from [PyTorch](https://pytorch.org/get-started/locally).

Install ```torch_sparse``` by following the Instruction from [pytorch_sparse](https://github.com/rusty1s/pytorch_sparse).

Install ```torch_geometric``` by following the Instruction from [torch_geometric](https://pytorch-geometric.readthedocs.io/en/latest/notes/installation.html).

Install ```scikit-learn``` by following the Instruction from [scikit-learn](https://scikit-learn.org/stable/getting_started.html).

Install ```networkx``` by following the Instruction from [networkx](https://networkx.org/documentation/stable/install.html).

Install ```optuna``` by following the Instruction from [optuna](https://optuna.org/#installation).

Install ```tqdm``` by following the Instruction from [tqdm](https://github.com/tqdm/tqdm).

## Instruction_to_Run_DeMinify

1. Download the dataset and save it in ```../DeMinify/data``` folder.

2. Download the DeMinify source code and run ```main.py``` to see the result for our experiment. 

