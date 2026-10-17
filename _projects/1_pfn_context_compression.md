---
layout: page
title: Context compression and adaptation in PFNs
description: How much in-context data does TabPFN need, and do LoRA-specialised models transfer across priors? Trust Lab, IIT Bombay.
importance: 1
category: research
---

**Trust Lab, IIT Bombay, May – July 2026.** Advisor: Prof. Pratik Jawanpuria (C-MInDS).

Prior-data fitted networks (PFNs) such as TabPFN make predictions in context: the training set is passed to a pretrained transformer together with the query points, and the prediction comes from a single forward pass. This project asked two questions:

1. **How much in-context data does TabPFN need?** I built a pipeline that extracts TabPFN's internal attention distributions and uses them to rank training samples by informativeness, so that inference can run on a compressed context.
2. **Do LoRA-specialised models transfer across priors?** I fine-tuned LoRA adapters on a frozen TabPFN across synthetic priors from four data-generating families. Cross-prior transfer degraded as the Wasserstein/MMD distance between priors grew.

I then related the geometry of the priors to the geometry of the adapters using adapter-similarity metrics, and tested the relationship with cross-family ablations. Along the way I found and corrected an undertraining artifact that had been inflating the effect.

**Tools:** PyTorch, TabPFN, LoRA.
