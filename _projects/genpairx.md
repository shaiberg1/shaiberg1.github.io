---
layout: page
title: GenPairX
description: A hardware-algorithm co-designed accelerator for paired-end read mapping.
img: assets/img/projects/genpairx.png
importance: 1
category: Systems for AI &amp; genomics
---

Read mapping — aligning sequenced DNA fragments to a reference genome — is a major
bottleneck in genome analysis because of expensive dynamic-programming alignment, and
existing filters handle the dominant paired-end reads poorly by evaluating each read of
a pair independently. **GenPairX** is a hardware-algorithm co-designed accelerator that
introduces a filter jointly considering both reads in a pair for far higher filtering
effectiveness, plus a lightweight alignment algorithm that replaces most costly dynamic
programming, backed by two specialized hardware mechanisms. It achieves orders of
magnitude higher throughput-per-watt than leading CPU-based mappers and 1.43&times; over
the best accelerator-based mapper, with no loss of accuracy.

Published at IEEE HPCA 2026.
