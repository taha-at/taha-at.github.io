---
title: "Numerical Solution of the 2D Incompressible Navier–Stokes Equations"
excerpt: "Lid-driven cavity flow solver using a fractional-step method on a MAC staggered grid (Re = 400, 1000, 3200).<br/><a href='/files/PDE_project.pdf'>Read the report (PDF)</a>"
collection: portfolio
permalink: /projects/navier-stokes-2d-cavity/
---

## Overview
This project solves the 2D incompressible Navier–Stokes equations for the **lid-driven cavity** benchmark using a **fractional step method** on a **staggered (MAC) grid**. Pressure is obtained from a Poisson equation (solved efficiently via DCT). The solver is validated against **Ghia et al. (1982)** centerline benchmarks.

## Highlights
- Staggered (MAC) grid for stable pressure–velocity coupling  
- Projection method: predictor → pressure Poisson → velocity correction  
- Tests at **Re = 400, 1000, 3200**  
- Validation vs. Ghia et al.

## Code
- The code is available on <a href="https://github.com/Hacker1one/navier-stokes-lid-driven-cavity-fractional-step">GitHub</a>


## Report
<iframe src="/files/PDE_project.pdf" width="100%" height="900px" style="border:none;"> </iframe>
