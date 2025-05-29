<h1 align="center">Niels Raunkjær Holm — Project Portfolio</h1>

<p align="center">
A selection of my projects in machine learning.<br>
</p>

---

## Table of Contents

* [How Low Can You Go? *(ICLR 2025)*](#how-low-can-you-go-iclr‑2025)
* [Inducing Point Laplace Approximations](#inducing-point-laplace-approximations)
* [Contrastive Pretraining for Combinatorial Optimization](#contrastive-pretraining-for-combinatorial-optimization)
* [Computing Geodesics on a Latent Manifold](#computing-geodesics-on-a-latent-manifold)

### 📫 Contact
|**Email** |**LinkedIn** |
| --------------- | ----------------------------------------------------- |
| [nielsraunkjaer@gmail.com](mailto:nielsraunkjaer@gmail.com) | [linkedin.com/in/nielsrh](https://www.linkedin.com/in/nielsrh) |

---

## $\bigstar$ How Low Can You Go? *(ICLR 2025)*

[Paper ↗](https://openreview.net/pdf?id=V71ITh2w40)

> **TL;DR** We investigate the intrinsic dimensionality of real world graphs by constructing procedures for losslessly embedding them in a metric space (e.g. Euclidean, Hyperbolic) based on a reconstruction objective function.

**Highlights**

* 2-stage procedure for losslessly embedding super large graphs, by utilizing the metric properties of our embedding space (since we can do linearithmic nearest neighbor search).
* Algorithm for searching for an upper bound of the lowest possible exact embedding dimension (intrinsic dimensionality).
* Theoretical proof that our metric latent distance model can losslessly embed in lower dimension than previous logistic PCA-based model.

---

## $\bigstar$ Inducing Point Laplace Approximations

*M.Sc. thesis - Work In Progress!*

> **TL;DR** A scalable Linearized Laplace Approximation for Bayesian Neural Networks, leveraging inducing points optimized via matrix free variational methods.

* Approximates the Generalized Gauss-Newton matrix for $N$ data points as $\sum_N \mathbf{J}^T \mathbf{J} \approx \sum_M \mathbf{J}^T \mathbf{J}$ with $M$ inducing points, where $M \ll N$.
* Derived a matrix free variational objective function for variational optimization of the inducing points, and implemented it in JAX.
* Derived a matrix free sampling method for posterior parameter and -predictive distribution inference, also implemented in JAX.

---

## $\bigstar$ Contrastive Pretraining for Combinatorial Optimization

[Report ↗](contrastive_pretraining_for_combinatorics.pdf)

> **TL;DR** We show that contrastive self‑supervised training on synthetic graphs has a subtle failure mode on a downstream maximum independent set task that on the surface looks like -almost- state-of-the-art performance.

**Highlights**

* Project on investigating pretraining procedures for graph neural networks, evaluating the quality of their learned representations on simple classification metrics and in a downstream NP hard combinatorial optimization problem (Maximum independent set).
* Made a critical discovery about the decoding algorithm; when coupled with models with poor representations, the entire pipeline reduced to a greedy decoder, misleadingly giving state-of-the-art results on many real-world test datasets.
* Ablated the findings with Exphormer, GCNN, GAT architectures.

---

## $\bigstar$ Computing Geodesics on a Latent Manifold

*Report is hosted on Google Drive to not share solutions to the DTU course project.*.

> **TL;DR** Investigation of Fisher–Rao geodesics in the latent space as a tool to improve identifiability in deep latent variable models (VAE \& VAE ensemble). Project in the DTU course [02460] Advanced Machine Learning.

**Highlights**

* Our implementation computed discretized curves in latent space that approximated Fisher-Rao geodesics - i.e. shortest distance in a space of probability distributions.
* We demonstrated that the VAE ensembles exhibited lower coefficient of variation ($\frac\mu\sigma$) than the single decoders.
* The trajectories between real data points also became closer to other embedded data points as we increased number of VAE decoders in the ensemble, indicating that the aggregated latent space more closely represented the data manifold.

---

<p align="center">
Last updated May 29, 2025
</p>
