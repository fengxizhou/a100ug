# Palmetto NVIDIA DGX A100 User Guide

This document provides a quick user guide on using the NVIDIA DGX A100 nodes on the Palmetto cluster.

## NVIDIA DGX A100

NVIDIA DGX A100 is a computer system built on NVIDIA A100 GPUs for AI workload. For more details, please check the [NVIDIA DGX A100 web Site](https://www.nvidia.com/en-us/data-center/dgx-a100/).

## Request a DGX A100 Node

On Palmetto, the DGX A100 nodes are integrated into the PBS resource and workload manager. An authorized user should request a DGX A100 Node using a `qsub` command in one the following ways:

1. Request a DGX A100 node in the interactive mode
   `qsub -I -l select=1:ncpus=20:mem=20gb:ngpus=1:gpu_model=p100:interconnect=10ge,walltime=5:00:00`
1. Request a DGX A100 node in the batch mode
   ``qsub -I -l select=1:ncpus=20:mem=20gb:ngpus=1:gpu_model=p100:interconnect=10ge,walltime=5:00:00`

  
