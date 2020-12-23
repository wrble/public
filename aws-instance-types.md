## AWS Instance Type Cheat Sheet

Cache invalidation and naming things - AWS has certainly had a hard time of the latter. Between the variety of instance types they offer and how long they're been around, there’s no consistency.

Whether starting a new service to run internally or reviewing something we have going, it’s always a struggle to find the right instance type for the needs. For example, there are three families (r, x, z) that optimize RAM in various ways in various combinations yet I always forget about the x and z variants. 

So I put together this "cheat sheet" for us internally and thought I'd share here for anyone else to use; pull requests welcome for updates. 

NOTE: Each vCPU is a thread of an Intel or AMD core, except where noted.

### Family Overview

* [a](#a): First generation graviton Arm processors, use [m6g](#m6g), [c6g](#c6g), or [r6g](#r6g) instead.
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

First generation graviton Arm processors, use [m6g](#m6g), [c6g](#c6g), or [r6g](#r6g) instead.

#### Variants

`a1` <a name="a1"></a>64-bit Arm Neoverse cores


## C

Compute-optimized with various core types.

#### Variants


`c4` <a name="c4"></a>Intel Xeon E5-2666 v3 cores

`c5` <a name="c5"></a>Xeon Platinum 8000 cores

`c5ad` <a name="c5ad"></a>c5a + locally attached SSD

`c5d` <a name="c5d"></a>c5 + locally attached SSD

`c5n` <a name="c5n"></a>c5 + optimized network

`c6g` <a name="c6g"></a>Arm-based AWS Graviton2 *vCPU is physical core

`c6gd` <a name="c6gd"></a>c6g with locally attached SSD storage



## D

Locally attached spinning HDD.

#### Variants

`d2` <a name="d2"></a>Attached spinning HDD

`d3en` <a name="d3en"></a>High-throughput w/attached spinning HDD


## F

FPGAs to run ASICs.

#### Variants

`f1` <a name="f1"></a>Attached FPGA and SSD


## G

GPUs for graphics or machine-learning.

#### Variants

`g3` <a name="g3"></a>Attached NVIDIA Tesla M60 GPU

`g4ad` <a name="g4ad"></a>Attached AMD Radeon Pro V520 GPU

`g4dn` <a name="g4dn"></a>Attached NVIDIA T4 Tensor Core GPU


## H

FAMILYDESC

#### Variants

`h1` <a name="h1"></a>Up to 16TB of spinning HDD.


## I

High-throughput local SSD.

#### Variants


`i3` <a name="i3"></a>Attached NVMe SSD

`i3en` <a name="i3en"></a>Larger SSDs and enhanced networking

`inf1` <a name="inf1"></a>AWS Inferentia for machine learning


## M

General-purpose with balanced memory, CPU, and storage.

#### Variants


`m4` <a name="m4"></a>Balanced, older Intel Xeon cores, use [m5](#m5) or [m6g](#m6g) instead

`m5` <a name="m5"></a>Balanced CPU and memory, latest Intel Xeon cores

`m5a` <a name="m5a"></a>Balanced CPU and memory, latest AMB EPYC cores

`m5ad` <a name="m5ad"></a>m5a with attached SSD

`m5d` <a name="m5d"></a>m5 with attached SSD


`m5n` <a name="m5n"></a>m5 with faster networking

`m5zn` <a name="m5zn"></a>m5n with highest 4.5GHz core speed

`m6g` <a name="m6g"></a>Balanced CPU and memory, latest Amazon Graviton 2 cores

`m6gd` <a name="m6gd"></a>m6g with attached SSD storage


## P

FAMILYDESC

#### Variants

`p2` <a name="p2"></a>NVIDIA K80 GPUs

`p3` <a name="p3"></a>NVIDIA Tesla V100 GPUs

`p4` <a name="p4"></a>NVIDIA A100 Tensor GPUs


## R

Memory-optimized.

#### Variants


`r4` <a name="r4"></a>Older high memory, use [r5](#r5) or [r6g](#r6g) instead.

`r5` <a name="r5"></a>Latest high memory, Intel Xeon cores

`r5a` <a name="r5a"></a>Latest high memory, AMD EPYC cores

`r5ad` <a name="r5ad"></a>r5a with attached SSD

`r5b` <a name="r5b"></a>r5 with optimized EBS

`r5dn` <a name="r5dn"></a>r5n with added SSD

`r5n` <a name="r5n"></a>r5 with faster networking

`r6g` <a name="r6g"></a>Latest high memory, Amazon Graviton 2 cores

`r6gd` <a name="r6gd"></a>r6g with attached SSD


## T

Burstable instances that will throttle after a CPU budget.

#### Variants


`t2` <a name="t2"></a>Older burstable instances *vCPU is physical core, use [t3](#t3) or [t4g](#t4g) instead

`t3` <a name="t3"></a>Latest generation, burstable instances with Intel Xeon cores

`t3a` <a name="t3a"></a>Latest generation, burstable instances with AMD EPYC cores

`t4g` <a name="t4g"></a>Latest generation, burstable instances with Amazon Graviton 2 cores


## X

Lowest price-per-GB RAM instances.

#### Variants

`x1` <a name="x1"></a>Memory-optimized Intel Xeon E7-8880 v3

`x1e` <a name="x1e"></a>x1 with optimized EBS


## Z

Highest core frequency with a lot of RAM.

#### Variants

`z1d` <a name="z1d"></a>Fast single core performance with really large CPU and memory configurations
