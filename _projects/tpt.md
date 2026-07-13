---
layout: page
title: Translation Pass-Through (TPT)
description: Near-native paging for VMs with one-dimensional page tables.
img: assets/img/projects/tpt.png
importance: 4
category: Systems &amp; storage
---

Address translation for VMs with large working sets is expensive: nested paging pays a
worst-case cost that grows with page-table depth, while shadow and paravirtualized
paging incur heavy hypervisor intervention on every guest page-table update.
**Translation Pass-Through** lets a VM directly control guest-virtual to host-physical
translation through one-dimensional page tables, while the host enforces inter-VM
isolation using new commodity-CPU support for physical-memory tagging. Prototyped in
KVM/QEMU with an enlightened Linux guest, TPT reaches native performance on real
data-center applications — up to 2.4&times; faster than nested and 1.4&times; faster
than shadow paging.

Published at USENIX ATC 2023.
