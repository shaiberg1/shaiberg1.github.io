---
layout: page
title: PACER
description: IO-aware power efficiency for ARM-based all-flash storage servers.
img: assets/img/projects/pacer.png
importance: 7
category: Systems &amp; storage
---

On-premise storage servers account for a large share of data-center power, yet
power-efficiency research has largely targeted compute and accelerators rather than
storage. **PACER** is a power-saving subsystem for ARM-based all-flash storage servers
that, unlike conventional CPU governors, is guided by storage-specific I/O metrics: it
monitors the server's operational state and predicts the performance impact of
power-saving actions, staying within configurable tolerance bounds. On real-world
traces it achieves 1.23&times; higher IOPS/watt than the native system, with power
savings on MLPerf Storage workloads at no performance cost.

Published at IEEE MSST 2024.
