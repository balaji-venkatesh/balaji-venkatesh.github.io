---
title: Publications
permalink: publications
layout: page
---

## Jack of All Scales: A Versatile FPGA Tensor Block for MXFP Precisions

Marwan Mekhemer, Ahmed Elsousy, Balaji Venkatesh, Raphael Rowley, Vaughn Betz, Nachiket Kapre, Andrew Boutros

2026 International Conference on Field-Programmable Logic and Applications | Gent, Belgium | Sep 2026

Modern deep learning workloads increasingly rely on narrow numerical formats to improve efficiency and reduce memory footprint. The recently standardized microscaling floating-point (MXFP) family of formats, including MXFP8, MXFP6, and MXFP4, offers a practical approach to low-precision inference, yet the digital signal processing (DSP) blocks in current FPGA architectures offer limited native support for these formats. We propose targeted modifications to the Altera Agilex-5 FPGAs' DSP block's internal tensor-mode architecture that enable native support for all MXFP precisions while retaining backward compatibility. Our results demonstrate a geometric mean throughput improvement of 5.4$\times$ across all MXFP formats.

## Accelerating Belief Propagation with Task-Based Hardware Parallelism

Balaji Venkatesh, Leo Han, Mark Jeffrey

2025 IEEE Canadian Conference on Electrical and Computer Engineering | Vancouver, Canada | May 2025 <br>
2024 Engineering Science Thesis at the University of Toronto | Toronto, Canada | Apr 2024

This project is the convergence of two directions, the first being innovations in residual belief propagation. Belief propagation is an algorithm used to compute statistical inferences on graphs called probabilistic graphical models. Applications include stereo image depth estimation, workplace safety, and healthcare patient experience. The second direction is hardware support for priority-ordered algorithms through task-based parallelism. This work implements belief propagation on an FPGA-based speculative parallel accelerator and demonstrates the possibility of increased performance.

DOI: 10.1109/CCECE64018.2025.11364448

[IEEE Xplore Listing](https://doi.org/10.1109/CCECE64018.2025.11364448)

[CCECE 2025 Paper PDF](./assets/ccece2025-paper.pdf)

[CCECE 2025 Slides PDF](./assets/ccece2025.pdf)

[UofT BASc Thesis PDF](./assets/bv-basc-thesis.pdf)

[Source Code on GitHub](https://github.com/balaji-venkatesh/chronos_rbp_hls)

## Automation of Thermal Energy Storage for Homes using Artificial Neural Networks

Balaji Venkatesh

2020 IEEE Canadian Conference on Electrical and Computer Engineering | London, Canada | Sep 2020

About 60% of the energy consumed by homes in North America is for air conditioning. Residential solar energy is now more cost effective; however, solar energy availability and air conditioning needs are mismatched in time, necessitating energy storage. In previous works, storage of energy in thermal air mass of homes has been proposed, and in this work, an artificial-neural-network-based thermostat is proposed. A method to train the model for an average home is demonstrated with an example and is shown to be effective. <br>

DOI: 10.1109/CCECE47787.2020.9255680

[IEEE Xplore Listing](https://doi.org/10.1109/CCECE47787.2020.9255680)

## Thermal Energy Storage for Homes

Balaji Venkatesh

2018 IEEE International Conference on Smart Energy Grid Engineering | Oshawa, Canada | Aug 2018

Conventional solar power solutions for homes convert solar energy using photovoltaic (PV) panels and then store the energy in batteries. However, batteries are expensive and environmentally unfriendly. Thermal Energy Storage for Homes (TESH) is a solution to mismatched timing of solar energy and home energy demand. By altering the temperature of the air mass in a home to store thermal energy, one can avoid the need for other forms of energy storage. This makes solar energy an even more environmentally friendly alternative energy source, while simultaneously reducing the cost of infrastructure. The proposed method was implemented as a prototype and tested. Test results are reported and discussed. <br>

DOI: 10.1109/SEGE.2018.8499511

[IEEE Xplore Listing](https://doi.org/10.1109/SEGE.2018.8499511) 

[SEGE 2018 Slides PDF](./assets/sege2018-slides.pdf)

[YRSTF 2017 Poster](./assets/yrstf2017-poster.pdf)