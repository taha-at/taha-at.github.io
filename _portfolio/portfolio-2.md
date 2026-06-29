---
title: "Design and Analysis of a Video Compression System"
excerpt: "Implementation and parameter optimization of a DCT-based video codec featuring block-matching motion estimation and parametric quantization.<br/><a href='/files/Video_compression_standard.pdf'>Read the report (PDF)</a>"
collection: portfolio
permalink: /projects/video-compression-system/
---

## Overview
This project focuses on the implementation and structural optimization of a custom video compression pipeline using Discrete Cosine Transform (DCT) spatial decorrelation, inter-frame motion estimation, and modern entropy coding architectures. Through rigorous experimentation across multiple pipeline variables, we analyze non-linear trade-offs between mathematical data fidelity (PSNR/MSE), computational throughput, and data compaction metrics (Compression Ratio).

## Highlights
- **Hybrid Video Architecture:** Implementation of a standard temporal/spatial pipeline processing sequential intra frames (I-frames) via pure block-level DCT quantization alongside inter frames (P-frames) derived from motion-compensated residual matrices.
- **Parametric Quantization Selection:** Comparison of H.264/AVC standard matrix layouts against custom Human Visual System (HVS) weight structures optimized for empirical contrast sensitivity models.
- **Adaptive Entropy Architectures:** Performance profiling of variable-length Huffman codes against true range-restricted Arithmetic Coding, confirming an absolute efficiency increase of 1–2% approaching the absolute source entropy limit.
- **Motion Estimation Optimization:** Parametric evaluation of localized Sum of Absolute Differences (SAD) block-matching algorithms. Results demonstrate diminishing utility returns beyond an absolute spatial search range threshold of 8 pixels.
- **Empirical Co-design Results:** Identification of optimal global baseline variables featuring an $8\times8$ pixel pixel transformation block size, a baseline scaling multiplier of $\sigma = 1.0$, and range-restricted adaptive arithmetic serialization tables.

## Code
- The code is available on <a href="https://github.com/ta/video-compression-codec-analysis">GitHub</a>

## Report
<iframe src="/files/Video_compression_standard.pdf" width="100%" height="900px" style="border:none;"> </iframe>
