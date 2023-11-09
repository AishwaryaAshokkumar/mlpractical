# MLP Compute Engines Tutorials Branch

A short code repo that guides you through the process of running experiments on the MLP Cluster and on the Google Cloud Platform.

## Why do I need it?
Most Deep Learning experiments require a large amount of compute as you have noticed in term 1. Usage of GPU can accelerate experiments around 30-50x therefore making experiments that require a large amount of time feasible by slashing their runtimes down by a massive factor. For a simple example consider an experiment that required a month to run, that would make it infeasible to actually do research with. Now consider that experiment only requiring 1 day to run, which allows one to iterate over methodologies, tune hyperparameters and overall try far more things. This simple example expresses one of the simplest reasons behind the GPU hype that surrounds machine learning research today.

## Introduction

The material available includes tutorial documents and code, as well as tooling that provides more advanced features to aid you in your quests
to train lots of learnable differentiable computational graphs.

## Getting Started

### Google Cloud Platform

Google Cloud Platform (GCP) is a cloud computing service that provides a number of services, including the ability to run virtual machines (VMs) on their infrastructure. The VMs are called Compute Engine instances. 

As a MLP course student, you will be given 50$ worth of credits. This is enough to run a number of experiments on the cloud.

To get started with GCP, please read the [this getting started guide](notes/google_cloud_setup.md).

The guide will take you through the process of setting up a GCP account, creating a project, creating a VM instance, and connecting to it. The VM instance will be a GPU-endowed Linux machine that already includes the necessary PyTorch packages for you to run your experiments. 

### MLP Cluster 

The MLP Cluster is a cluster consisting of server rack machines, each equipped with 8 x NVIDIA 1060 Ti GTX GPUs. Currently there are 200 GPUs available for use. The system is managed using the open source cluster management software named [Slurm](https://slurm.schedmd.com/overview.html). Slurm has various advantages over the competition, including full support of GPU resource scheduling.

The cluster can be accessed via SSH from a DICE machine or from your own machine if you established a remote connection.

To get started with the MLP Cluster, please read the [this getting started guide](notes/mlp_cluster_quick_start_up.md).

The guide will take you through the process of setting up your environment, installing the necessary packages, and submitting your first job to the cluster.
