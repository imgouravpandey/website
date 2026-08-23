---
title: "Karpenter Alternative Scheduler"
date: 2025-03-01
featured: true
tags: ["kubernetes", "karpenter", "scheduling", "internal-product"]
description: "Built an internal scheduler through 14 iteration cycles that solves the pod over-provisioning problem that Karpenter misses."
---

Karpenter efficiently provisions nodes to match pod requests, but if developers request 4 CPUs for a pod that uses 0.2 CPUs, Karpenter will buy a node to fit that bloated request. It bin-packs waste, but it cannot fix the waste itself.

Built an internal scheduling component that optimizes at the scheduling stage itself, not just at provisioning. Ran 14 internal iteration cycles to find the optimal bin-packing strategy that accounts for actual resource utilization, not just requested resources.

**Tools:** Kubernetes internals, Go, EKS, Karpenter
