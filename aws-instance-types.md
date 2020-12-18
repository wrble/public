## AWS Instance Type Cheat Sheet

NOTE: Each vCPU is a thread of an Intel or AMD core, except where noted.

### Family Overview

* [a](#a): First generation graviton Arm processors.
* [c](#c): Compute-optimized with various core types.
* [d](#d): Locally attached spinning HDD.
* [f](#f): FPGAs to run ASICs.
* [g](#g): GPUs for graphics or machine-learning.
* [i](#i): High-throughput local SSD.
* [m](#m): General-purpose with balanced memory, CPU, and storage.
* [r](#r): Memory-optimized.
* [t](#t): Burstable instances that will throttle after a CPU budget.
* [x](#x): Lowest price-per-GB RAM instances.
* [z](#z): Highest core frequency with a lot of RAM.

## A

First generation graviton Arm processors.

### Variants

`a1` OLD: 64-bit Arm Neoverse cores


## C

Compute-optimized with various core types.

### Variants


`c4` Intel Xeon E5-2666 v3 cores

`c5` Xeon Platinum 8000 cores

`c5ad` c5a + locally attached SSD

`c5d` c5 + locally attached SSD

`c5n` c5 + optimized network

`c6g` Arm-based AWS Graviton2 *vCPU is physical core

`c6gd` c6g with locally attached SSD storage



## D

Locally attached spinning HDD.

### Variants

`d2` Attached spinning HDD

`d3en` High-throughput w/attached spinning HDD


## F

FPGAs to run ASICs.

### Variants

`f1` Attached FPGA and SSD


## G

GPUs for graphics or machine-learning.

### Variants

`g3` Attached NVIDIA Tesla M60 GPU

`g4ad` Attached AMD Radeon Pro V520 GPU

`g4dn` Attached NVIDIA T4 Tensor Core GPU


## I

High-throughput local SSD.

### Variants


`i3en` Attached NVMe SSD

`inf1` AWS Inferentia for machine learning


## M

General-purpose with balanced memory, CPU, and storage.

### Variants


`m4` Balanced, older Intel Xeon cores

`m5` Balanced CPU and memory, latest Intel Xeon cores

`m5a` Balanced CPU and memory, latest AMB EPYC cores

`m5ad` m5a with attached SSD

`m5d` m5 with attached SSD


`m5n` m5 with faster networking

`m5zn` m5n with highest 4.5GHz core speed

`m6g` Balanced CPU and memory, latest Amazon Graviton 2 cores

`m6gd` m6g with attached SSD storage


## R

Memory-optimized.

### Variants


`r4` Older high memory

`r5` Latest high memory, Intel Xeon cores

`r5a` Latest high memory, AMD EPYC cores

`r5ad` r5a with attached SSD

`r5b` r5 with optimized EBS

`r5dn` r5n with added SSD

`r5n` r5 with faster networking

`r6g` Latest high memory, Amazon Graviton 2 cores

`r6gd` r6g with attached SSD


## T

Burstable instances that will throttle after a CPU budget.

### Variants


`t2` Burstable instances *vCPU is physical core

`t3` Latest generation, burstable instances with Intel Xeon cores

`t3a` Latest generation, burstable instances with AMD EPYC cores

`t4g` Latest generation, burstable instances with Amazon Graviton 2 cores


## X

Lowest price-per-GB RAM instances.

### Variants

`x1` Memory-optimized Intel Xeon E7-8880 v3

`x1e` x1 with optimized EBS


## Z

Highest core frequency with a lot of RAM.

### Variants

`z1d` Fast single core performance with really large CPU and memory configurations
