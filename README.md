# InCor-RKM - Informative Core Sampling for Scalable Restricted Kernel Machines

This repository contains the MATLAB implementation corresponding to the paper:

Anuradha Kumari, Johan Suykens, and M. Tanveer (2026), Informative Core Sampling for Scalable Restricted Kernel Machines, Neural Networks, Elsevier (Revision Submitted).

If you use this code in your work, please cite the above paper appropriately.
For any issues or bugs, please contact: anuradhaiitg123@gmail.com
 

This repository provides implementations of four proposed scalable RKM models.

The implemented models are:

# InCor-RKM: Informative core sampled restricted kernel machine

# RKM-RAFT: Restricted kernel machine with randomized Fourier features and approximate factorization technique 

# RKMRF: RKM with random Fourier features

# RKMRF-S: RKM with RFF and sampling


Train.txt / Test.txt corresponds to example training and testing datasets.

# Folder Descriptions
1. InCor-RKM

Files:
InCor_RKM_main.m: Main file for executing InCor-RKM.
InCor_RKM_classification.m: Function implementing the classification process using informative cores.
InCor.m: Implements informative core selection procedure.
compute_kernel_matrix.m: Computes kernel matrix for given data.

Usage:
Run InCor_RKM_main.m after setting hyperparameters such as kernel width, number of cores, and regularization constants.


2. RKM-RAFT

Files:
RKM_RAFT_main.m: Main driver script for RKM-RAFT.
RKM_RAFT_classification.m: Core classification algorithm using randomized SVD.
compute_kernel_matrix.m: Kernel computation function.
randomizedSVD.m / solve_with_svd.m: Utility functions for randomized matrix decomposition and efficient solving.

Usage:
Execute RKM_RAFT_main.m to train and test the model. Configure parameters kernel parameter, and regularization constants.

3. RKMRF

Files:
RKMRF_main.m: Main file for RKMRF model.
RKMRF_classification.m: Function implementing RKM classification using representative features.
compute_kernel_matrix.m: Kernel computation routine.
Train.txt / Test.txt: Sample datasets.

Usage:
Run RKMRF_main.m to perform training and evaluation. 

4. RKMRF-S

Files:
RKMRFS_main.m: Main file for RKMRFS model.
RKMRFS_classification.m: Implements sparse variant of RKMRF model.
compute_kernel_matrix2.m: Modified kernel computation supporting sparse structure.

Usage:
Execute RKMRFS_main.m directly.

General Instructions

Load or replace Train.txt and Test.txt with your dataset.

Set parameters such as kernel type, kernel width, regularization parameters, and number of informative cores (if applicable).

Run the main script corresponding to the desired model.

The scripts will output:

Classification accuracy

Training time

(Optionally) model parameters and core indices




