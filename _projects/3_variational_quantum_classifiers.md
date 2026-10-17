---
layout: page
title: Variational quantum classifiers
description: PennyLane variational quantum classifiers benchmarked against classical baselines. Quantum Computing Group, IIT Roorkee.
img: assets/img/projects/qml_roc_breast_cancer.png
importance: 3
category: projects
github: https://github.com/para-bellum-hub/qml_classifier
---

**Quantum Computing Group, IIT Roorkee, December 2025 – January 2026.** Code: [para-bellum-hub/qml_classifier](https://github.com/para-bellum-hub/qml_classifier).

I built variational quantum classifiers (VQCs) in PennyLane, using a data re-uploading ansatz with circular CNOT entanglement, and trained them with a class-weighted loss, early stopping on validation AUC, stratified splits, and feature scaling fitted on the training split only. Each classifier was compared against logistic regression and a random forest on the same splits.

| Dataset                                 |  VQC  | Logistic regression | Random forest |
| :-------------------------------------- | :---: | :-----------------: | :-----------: |
| Credit-card fraud (100k rows, 4 qubits) | 0.959 |        0.960        |     0.979     |
| Breast cancer (scikit-learn)            | 0.960 |        0.965        |     0.970     |

_Test-set ROC-AUC._ On both datasets the VQC is close to logistic regression and below the random forest.

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/projects/qml_roc_breast_cancer.png" title="ROC curves, breast-cancer dataset" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    ROC curves on the breast-cancer test set: VQC (blue), logistic regression (orange), random forest (green).
</div>
