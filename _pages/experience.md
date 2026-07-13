---
layout: page
title: experience
permalink: /experience/
description: Where I have worked and studied.
nav: true
nav_order: 3
---

<ul class="timeline">
  <li class="tl-item">
    <div class="tl-logo"><img src="{{ '/assets/img/logos/huawei.png' | relative_url }}" alt="Huawei"></div>
    <div class="tl-body">
      <div class="tl-org tl-org--head">Huawei Zurich Research Center</div>
      <ul class="tl-roles">
        <li>
          <div class="tl-rolehead"><span class="tl-role">Principal Researcher · Team &amp; Technical Lead</span><span class="tl-date">May 2025 – present</span></div>
          <div class="tl-details">
            <p>Lead a research team at the intersection of storage and AI: storage systems that accelerate LLM inference and agentic-AI workloads, alongside CXL-based memory systems for modern data centers.</p>
            <p><span class="tl-ld">KV-cache systems for LLM inference.</span> Persist and reuse KV caches beyond exact prefix matches via selective recomputation of a small token fraction; offload caches across GPU memory, DRAM, and NVMe, managing bandwidth to sustain cache loading under concurrent inference — prototyped on vLLM, SGLang, and LMCache.</p>
            <p><span class="tl-ld">RAG serving.</span> Speculative decoding that drafts tokens from the retrieval datastore and verifies them in parallel on the target model, removing the separate draft model; approximate caching of retrievals across similar queries.</p>
            <p><span class="tl-ld">Systems for agentic AI.</span> New system interfaces and file systems for AI agents, including offloading agents’ data operations into storage (in-storage processing).</p>
          </div>
        </li>
        <li>
          <div class="tl-rolehead"><span class="tl-role">Senior Researcher</span><span class="tl-date">Aug 2023 – May 2025</span></div>
          <div class="tl-details">
            <p><span class="tl-ld">Distributed caching over memory fabrics.</span> Designed an OS-level distributed page cache for CXL&nbsp;3.0 shared memory that keeps a single DRAM copy of each file page across nodes while preserving POSIX semantics — up to 12.4× speedups in multi-host emulation.</p>
            <p><span class="tl-ld">UnifiedBus.</span> Contributed to the specification of UnifiedBus (UB), Huawei’s openly published interconnect for peer-to-peer resource pooling in SuperPoD-scale AI systems.</p>
            <p><span class="tl-ld">In-storage processing.</span> Accelerated approximate-nearest-neighbor vector search inside storage devices to cut data movement for retrieval and vector-database workloads.</p>
            <p><span class="tl-ld">MoE inference offload.</span> Enabled Mixture-of-Experts LLM inference on memory-constrained servers by offloading expert (FFN) weights to fast storage and streaming the experts activated per token.</p>
            <p><span class="tl-ld">Power-efficient storage servers.</span> Co-led an I/O-metric-guided CPU power-management subsystem (DVFS and core power-gating) for all-flash storage servers, improving IOPS per watt on production traces at no performance cost.</p>
            <p><span class="tl-ld">SMT scheduling.</span> Devised symbiosis-aware scheduling that co-locates threads with complementary resource profiles on SMT cores, raising throughput without hardware changes.</p>
          </div>
        </li>
      </ul>
    </div>
  </li>
  <li class="tl-item">
    <div class="tl-logo"><img src="{{ '/assets/img/logos/unifabrix.png' | relative_url }}" alt="UniFabrix"></div>
    <div class="tl-body">
      <div class="tl-role">Chief Architect, Advanced Technologies</div>
      <div class="tl-org">UniFabrix</div>
      <div class="tl-date">2022 – 2023</div>
      <div class="tl-details">
        <p><span class="tl-ld">CXL memory pooling.</span> Architected dynamic borrowing and lending of memory across hosts over CXL, built on Linux memory hot-plug; hardware/software co-design and OS support for disaggregated memory.</p>
        <p><span class="tl-ld">Performance frameworks.</span> Built frameworks that let applications consume pooled memory without performance loss — and with gains where the pool’s added bandwidth is exploited.</p>
      </div>
    </div>
  </li>
  <li class="tl-item">
    <div class="tl-logo"><img src="{{ '/assets/img/logos/imperial.svg' | relative_url }}" alt="Imperial College London"></div>
    <div class="tl-body">
      <div class="tl-role">Visiting Scholar</div>
      <div class="tl-org">Imperial College London</div>
      <div class="tl-date">2022</div>
      <div class="tl-details">
        <p>Designed a memory-virtualization mechanism that lets VMs manage flat guest-virtual-to-host-physical page tables, with inter-VM isolation enforced through per-VM physical-memory tagging repurposed from confidential-computing hardware; with Prof. Peter Pietzuch and Prof. Lluís Vilanova. Prototyped in Linux/KVM/QEMU on x86-64: near-native paging — up to 2.4× faster than nested paging (Intel EPT).</p>
      </div>
    </div>
  </li>
  <li class="tl-item">
    <div class="tl-logo"><img src="{{ '/assets/img/logos/technion.svg' | relative_url }}" alt="Technion"></div>
    <div class="tl-body">
      <div class="tl-role">Ph.D. &amp; Lecturer, Electrical &amp; Computer Engineering</div>
      <div class="tl-org">Technion — Israel Institute of Technology</div>
      <div class="tl-date">2017 – 2022</div>
      <div class="tl-details">
        <p>Ph.D. thesis “Memory Management for Emerging Memory Technologies in Future Data-Centers,” advised by Prof. Mark Silberstein.</p>
        <p><span class="tl-ld">Disaggregated memory &amp; storage.</span> A Linux memory-tiering subsystem for high-latency far memory (HotBox, ISMM ’22) and a redesign of the Linux swap subsystem for ZNS SSDs (ZNSwap, USENIX ATC ’22 / ACM TOS ’23).</p>
        <p><span class="tl-ld">Virtualization.</span> Near-native memory virtualization via guest-managed flat page tables with CPU physical-memory tagging (TPT, USENIX ATC ’23).</p>
        <p><span class="tl-ld">Teaching.</span> Lecturer and TA-in-charge for “Structure of Operating Systems”; mentored graduate students, including the nested-virtualization work that became HyperTurtle (Best Paper, USENIX ATC ’25).</p>
      </div>
    </div>
  </li>
  <li class="tl-item">
    <div class="tl-logo"><img src="{{ '/assets/img/logos/huawei.png' | relative_url }}" alt="Huawei"></div>
    <div class="tl-body">
      <div class="tl-role">Software Architect, Innovation Team</div>
      <div class="tl-org">Toga Networks — a Huawei Company</div>
      <div class="tl-date">2019 – 2021</div>
      <div class="tl-details">
        <p><span class="tl-ld">Consultant (2020–2021).</span> Architected memory management that removes memory-pinning for next-generation RDMA NICs: NIC-side on-the-fly address translation with page-fault handling and requester/responder memory-status signaling — three patent families (US and EP patents granted). Also designed efficient intra-host data movement for UCX.</p>
        <p><span class="tl-ld">Intern (2019).</span> Linux kernel memory-management development for HPC systems.</p>
      </div>
    </div>
  </li>
  <li class="tl-item">
    <div class="tl-logo"><img src="{{ '/assets/img/logos/logicblox.png' | relative_url }}" alt="LogicBlox"></div>
    <div class="tl-body">
      <div class="tl-role">Software Engineer, Runtime Team</div>
      <div class="tl-org">LogicBlox</div>
      <div class="tl-date">2016</div>
      <div class="tl-details">
        <p>Implemented and optimized vectorized (SIMD) query execution in the LogicBlox&nbsp;4 runtime — a commercial Datalog (LogiQL) database engine — and investigated GPU offload for accelerating query evaluation.</p>
      </div>
    </div>
  </li>
  <li class="tl-item">
    <div class="tl-logo"><img src="{{ '/assets/img/logos/amd.svg' | relative_url }}" alt="AMD"></div>
    <div class="tl-body">
      <div class="tl-role">Co-Op Engineer, Innovation Team</div>
      <div class="tl-org">AMD</div>
      <div class="tl-date">2015</div>
      <div class="tl-details">
        <p>Prototyped OS support for transparent peer-to-peer DMA between NVMe SSDs and GPUs with standard POSIX file semantics, removing the CPU from the data path — paving the way for later GPU-direct storage technologies such as NVIDIA GPUDirect Storage (GDS).</p>
      </div>
    </div>
  </li>
  <li class="tl-item">
    <div class="tl-logo"><img src="{{ '/assets/img/logos/technion.svg' | relative_url }}" alt="Technion"></div>
    <div class="tl-body">
      <div class="tl-role">M.Sc. &amp; Teaching Assistant, Electrical &amp; Computer Engineering</div>
      <div class="tl-org">Technion — Israel Institute of Technology</div>
      <div class="tl-date">2015 – 2017</div>
      <div class="tl-details">
        <p>Thesis “High-Performance Disk I/O on GPUs”: OS-integrated peer-to-peer DMA between NVMe SSDs and GPUs behind standard POSIX file I/O (SPIN, USENIX ATC ’17). TA-in-charge for “Structure of Operating Systems.” <em>Cum Laude</em> (thesis 95%, courses 96.7%).</p>
      </div>
    </div>
  </li>
  <li class="tl-item">
    <div class="tl-logo"><img src="{{ '/assets/img/logos/technion.svg' | relative_url }}" alt="Technion"></div>
    <div class="tl-body">
      <div class="tl-role">B.Sc., Electrical &amp; Computer Engineering</div>
      <div class="tl-org">Technion — Israel Institute of Technology</div>
      <div class="tl-date">2011 – 2015</div>
      <div class="tl-details">
        <p>Specialization in Computers (hardware &amp; software) and Networks. <em>Cum Laude</em> (average 90.2%).</p>
      </div>
    </div>
  </li>
</ul>

## Awards &amp; honors

<div class="awards-grid">
  <div>
    <div class="awards-h">Industry</div>
    <ul>
      <li><span><span class="aw-name">President’s Award</span> <span class="aw-org">· Significant Business Contribution, Huawei</span></span><span class="aw-year">2026</span></li>
      <li><span><span class="aw-name">Technology Innovation Award</span> <span class="aw-org">· Huawei</span></span><span class="aw-year">2026</span></li>
      <li><span><span class="aw-name">European Research Institute Excellent Contributor</span> <span class="aw-org">· Huawei</span></span><span class="aw-year">2025</span></li>
      <li><span><span class="aw-name">Future Star Award</span> <span class="aw-org">· Huawei (×2)</span></span><span class="aw-year">2024–2025</span></li>
      <li><span><span class="aw-name">Technical Innovation Award</span> <span class="aw-org">· Huawei</span></span><span class="aw-year">2024</span></li>
      <li><span><span class="aw-name">1st Place</span> <span class="aw-org">· Mellanox BlueField Hackathon</span></span><span class="aw-year">2019</span></li>
    </ul>
  </div>
  <div>
    <div class="awards-h">Academic</div>
    <ul>
      <li><span><span class="aw-name">Best Paper Award</span> <span class="aw-org">· USENIX ATC — <em>HyperTurtle</em></span></span><span class="aw-year">2025</span></li>
      <li><span><span class="aw-name">Outstanding Teaching Assistant</span> <span class="aw-org">· Technion (×5)</span></span><span class="aw-year">2016–2019</span></li>
      <li><span><span class="aw-name">M.Sc. &amp; B.Sc. <em>Cum Laude</em></span> <span class="aw-org">· Technion</span></span><span class="aw-year"></span></li>
      <li><span><span class="aw-name">Technion President’s List</span></span><span class="aw-year">2015</span></li>
    </ul>
  </div>
</div>
