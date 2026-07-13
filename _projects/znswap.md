---
layout: page
title: ZNSwap
description: Un-blocking OS swap by co-designing it with ZNS SSDs.
img: assets/img/projects/znswap.png
importance: 3
category: Systems &amp; storage
---

Swapping to conventional SSDs suffers from opaque flash management: the device's
own garbage collection runs uncoordinated with the OS, causing write amplification,
throughput cliffs, and poor isolation between tenants. **ZNSwap** redesigns the Linux
swap subsystem around Zoned Namespace (ZNS) SSDs, moving garbage collection into the
host and co-designing it with the kernel swap logic so the two share usage statistics
and correctly account for GC bandwidth. The result is stable throughput across access
patterns, up to 10&times; lower tail latency, and 5&times; higher throughput for an
in-memory key-value store.

Published at USENIX ATC 2022 and in ACM Transactions on Storage 2023.
