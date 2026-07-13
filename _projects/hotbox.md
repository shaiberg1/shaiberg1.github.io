---
layout: page
title: HotBox
description: Rethinking OS memory management for disaggregated memory.
img: assets/img/projects/hotbox.png
importance: 5
category: Systems &amp; storage
---

Tiered-memory optimizations were designed for local byte-addressable non-volatile
memory that is only a few times slower than DRAM. Disaggregated memory is far
slower, which undermines those well-established techniques. Through analysis of real
workloads, this work shows that disaggregation calls for different design choices, and
builds **HotBox**, a Linux disaggregated-memory management subsystem that maximizes the
local-memory hit rate with low overhead and only minor kernel changes — outperforming
state-of-the-art tiered-memory systems by up to 2.25&times; on memory-intensive
benchmarks.

Published at ACM SIGPLAN ISMM 2022.
