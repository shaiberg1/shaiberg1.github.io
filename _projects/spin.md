---
layout: page
title: SPIN
description: Peer-to-peer DMA between SSDs and GPUs, inside the OS file stack.
img: assets/img/projects/spin.png
importance: 6
category: Systems &amp; storage
---

GPUs can DMA data directly from NVMe SSDs to keep the CPU off the data path, but doing
so bypasses the OS file I/O layers and loses the page cache, read-ahead, and POSIX
consistency. **SPIN** integrates peer-to-peer DMA into the standard OS file I/O stack,
dynamically choosing between the P2P and page-cache paths, re-enabling read-ahead for
sequential access while preserving POSIX semantics and portability across GPUs and
SSDs. It exceeds raw P2P throughput by up to an order of magnitude and speeds real
GPU-accelerated applications by 2.6&ndash;3.3&times;.

Published at USENIX ATC 2017 and in ACM Transactions on Computer Systems 2019.
