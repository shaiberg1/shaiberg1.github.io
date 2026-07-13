---
layout: page
title: DPC
description: A single cluster-wide page cache over CXL — no replication.
img: assets/img/projects/dpc.png
importance: 1
category: Systems for AI &amp; genomics
---

Distributed file systems rely on uncoordinated per-node page caches that replicate hot
data across every node, wasting aggregate cluster DRAM and paying heavy coherence
overhead. **DPC** is an OS-level distributed page cache built on CXL 3.0 memory
semantics that treats all cluster DRAM as a single cache budget and enforces a
single-copy invariant: each file page has exactly one owner node holding the sole DRAM
copy, and other nodes reach it through CXL-based remote mappings rather than replicating
it. On a multi-host CXL 3.0 emulation framework, DPC delivers up to 12.4&times; speedup
and a 5.6&times; geometric-mean speedup on data-sharing workloads.

Preprint (arXiv:2604.19494), 2026.
