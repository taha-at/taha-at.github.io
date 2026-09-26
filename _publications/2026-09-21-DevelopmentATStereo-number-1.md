---
title: "Development of Abdelwahab-Taha Stereotactic Software for Neurosurgery Surgical Planning"
collection: publications
category: preprints
permalink: /publication/2026-09-21-development-of-abdelwahab-taha-stereotactic-software
excerpt: 'A source-available 3D Slicer planning module for frame-based stereotaxy and deep brain stimulation, providing sub-millimeter registration accuracy (0.40 ± 0.15 mm) and an approximate threefold reduction in planning workflow duration.'
date: 2026-09-21
venue: 'Research Square (Preprint)'
paperurl: 'https://doi.org/10.21203/rs.3.rs-11053911/v1'
codeurl: 'https://doi.org/10.5281/zenodo.22542855'
citation: 'Abdelrahman Taha, Youstina Mohsen, Yousef Mansour, Ahmed Nageeb Taha, Ahmed Abdulwahab. (2026). &quot;Development of Abdelwahab-Taha Stereotactic Software for Neurosurgery Surgical Planning.&quot; <i>Research Square</i>. doi:10.21203/rs.3.rs-11053911/v1.'
---

## Overview

In frame-based stereotaxy, planning software must map image-derived coordinates into the physical coordinate system of the stereotactic frame, tightly coupling software design to hardware geometry. Most existing commercial platforms are proprietary, cost-prohibitive, and hardware-restricted, limiting accessibility in resource-constrained surgical settings. 

**Abdelwahab–Taha Stereotactic (ATStereo)** is a source-available surgical planning toolkit built directly as a [3D Slicer](https://www.slicer.org/) extension and tailored specifically to the geometric configuration of the Abdelwahab stereotactic frame.

<Image src="image_agent_tag_16035675017575651172" alt="Stereotactic frame trajectory planning in 3D Slicer" caption="Frame-based stereotactic trajectory planning" />

---

## Key Features

* **3D Frame Kinematic Reconstruction:** Anchored to dual physically accessible reference origins for reliable spatial orientation.
* **Real-Time Fiducial Alignment:** Interactive landmark detection and CT/MRI coordinate transformation.
* **Bilateral Trajectory Planning:** Native integration with the DISTAL subcortical atlas for Deep Brain Stimulation (DBS) targeting and critical structure avoidance.
* **Open & Accessible:** Built as a free, extensible plugin on top of the open-source 3D Slicer medical imaging platform.

---

## Experimental Validation & Results

| Metric | Result | Context / Baseline |
| :--- | :--- | :--- |
| **Registration RMSE** | **0.40 ± 0.15 mm** | Strict < 1.0 mm quality control threshold (range: 0.12–0.94 mm) |
| **Workflow Time** | **1.86 ± 0.53 min** | ~3× faster than *BrainStereo*; stabilizes in 5–10 trials for novices |
| **Electrode Concordance** | **0.256 ± 0.072 mm** | Validated on clinical PD DBS cohorts (OpenNeuro `ds005906`) |
| **Safety Clearance** | **100%** | Zero vascular or critical structure violations across planned trajectories |

---

## Links & Resources

* **Preprint (Research Square):** [doi:10.21203/rs.3.rs-11053911/v1](https://doi.org/10.21203/rs.3.rs-11053911/v1)
* **Code & Data Archive (Zenodo):** [doi:10.5281/zenodo.22542855](https://doi.org/10.5281/zenodo.22542855)
