# The Measurement Operator Changes Which Bits Matter: Operator-Conditioned Mixed Precision for Inverse Vision

**Chaewon Yoon** · University of Wisconsin–Madison  
**IEEE/CVF Winter Conference on Applications of Computer Vision (WACV 2027), Algorithms Track · Accepted**

## Overview

A change in sensing geometry can alter which stages of an inverse-vision reconstruction model are most sensitive to reduced numerical precision, even when reconstruction difficulty is controlled.

This work introduces **Operator-Susceptibility Matching (OSM)**, which estimates stage-level precision sensitivity from the calibrated sensing operator and uses those estimates to select a mixed-precision schedule without exhaustive per-operator search.

## Results

The controlled eight-stage ProxSCI-8 study evaluates 256 binary precision schedules. At a budget of three high-precision stages, OSM achieves **2.7% mean normalized operator-visible regret**, compared with **6.3%** for the best global-static schedule.

In a separate native A100 timing evaluation, the selected mixed-precision configuration takes **16.4 ms** per reconstruction, compared with **23.6 ms** for the FP16 reference, a **1.44×** speedup. Reconstruction quality and native execution time are evaluated under different precision protocols.

## Research areas

Computational imaging · Inverse problems · Mixed-precision inference · Quantization · Efficient machine learning

## Citation

Chaewon Yoon. *The Measurement Operator Changes Which Bits Matter: Operator-Conditioned Mixed Precision for Inverse Vision.* Accepted to the IEEE/CVF Winter Conference on Applications of Computer Vision (WACV), 2027. Proceedings forthcoming.

[Copyable BibTeX](CITATION.md)

## Related research

This paper is part of my research on efficient and reliable machine learning under numerical precision and computational constraints. A related project studies [quantized defect correction in fractional neural operators](https://github.com/chaewon-research/qdc-fractional-neural-operators).
