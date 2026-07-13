---
layout: page
title: HyperTurtle
description: Accelerating nested virtualization with eBPF offload. Best Paper, USENIX ATC 2025.
img: assets/img/projects/hyperturtle.png
importance: 2
category: Systems &amp; storage
---

Nested virtualization provides strong isolation but pays a non-trivial cost dominated
by world switches between the bare-metal and nested layers; prior fixes are either
intrusive or give up control over the nested VMs. **HyperTurtle** offloads selected
critical-path parts of the nested hypervisor by encapsulating them as eBPF programs
that run safely in the bare-metal hypervisor context, cutting world switches while
retaining control and avoiding intrusive changes. Applied to memory management,
networking, and profiling, it delivers gains such as 5&times; faster EPT fault handling
and up to 27% faster Kata-container boot.

Received a **Best Paper Award** at USENIX ATC 2025.
