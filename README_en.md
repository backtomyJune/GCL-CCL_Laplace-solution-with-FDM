<p align="center">
  <a href="https://github.com/backtomyJune/GCL-CCL_Laplace-solution-with-FDM/blob/main/README.md/">中文</a>
  ｜
  <a href="https://github.com/backtomyJune/GCL-CCL_Laplace-solution-with-FDM/blob/main/README_en.md">English</a>
</p>

# GCL/CCL Liner Leakage Mechanism Analytical Solution Construction and Validation Platform
## Project Overview
This project aims to build a high-precision analytical solution and finite element solver platform for the leakage mechanism of composite clay liners.

- The core objective is to address the industry-wide challenge of insufficient accuracy in leakage assessment for landfill and contaminated site liner systems. By integrating theoretical innovation with experimental validation, it significantly enhances the accuracy and reliability of leakage prediction.
- The project provides a novel analytical solution for the Laplace equation in a circular domain under cylindrical coordinates, establishing a more precise two-dimensional seepage evaluation model.
- This platform is designed to offer a standardized, theoretically sound, and validated solution for predicting the long-term service performance of liners, material verification, and engineering design.
- Due to project and funding requirements, only part of the code is open-sourced for reference and learning.

If this project is helpful to you :thumbsup:, please give it a Star :star: in the upper right corner! Thank you!!
## Current Research Progress
Currently, the project has completed the derivation of the new analytical solution and is developing the finite element solver:
### :white_check_mark: Completed:
### 1. Theoretical Construction of Seepage Analytical Solution in Cylindrical Coordinates
Addressing the leakage problem of liner systems, the analytical solution for the Laplace equation in a circular domain under cylindrical coordinates was derived. This establishes a more accurate mathematical model for two-dimensional seepage assessment, laying a theoretical foundation for precise leakage prediction.
### 2. COMSOL Circular Domain Seepage Model and Parameterized Modeling via Secondary Development
Based on the derived analytical theory, a corresponding 2D axisymmetric finite element model was built in COMSOL Multiphysics to accurately represent the geometric structure and physical fields of the liner. Utilizing the open-source `mph` library (https://mph.readthedocs.io/en/1.2/) for secondary development, parameterized automated modeling and batch calculation were implemented, significantly improving multi-scenario simulation efficiency. This provides a reliable fully-numerical benchmark for validating the analytical solution and subsequent research.

## :children_crossing: Work in Progress
### 1. Model Optimization and Scenario Expansion
Further optimize the analytical solution model and explore its application in more complex boundary conditions and scenarios like unsaturated seepage to enhance the model's universality and precision.
### 2. Multi-Physical Field Coupled Model Integration
Plan to gradually integrate factors such as chemical gradients and mechanical deformation into the existing seepage model, exploring the establishment of a Hydro-Mechanical-Chemical (HMC) coupled analysis framework to more comprehensively characterize liner service performance.
### 3. Automated Assessment Toolchain Development
Develop an integrated automated toolchain or UI interface encompassing data processing, model calculation, result visualization, and report generation to improve platform usability and efficiency.

## Tech Stack
- Simulation: COMSOL Multiphysics (for multi-physics simulation and model secondary development)
- Programming Languages: Python, MATLAB (for machine learning model development, analytical solution calculation, data processing and analysis)
- Design & Modeling: CAD, 3DMAX (for test device design and 3D model construction)
- Data Visualization: Matplotlib, Origin, etc.

## Contact Me
- If you have any questions or collaboration intentions, please contact via:
- Email: 2311110061@nbu.edu.cn / 289176263@qq.com

## Acknowledgments
- Thanks to the funding from the supervisor's National Natural Science Foundation of China (Grant Nos. 42477151; 42107174), China Postdoctoral Science Foundation (Grant No. 2023M743058), Zhejiang Provincial Natural Science Foundation Key Project (LZ25E080009), and Zhejiang Provincial Postdoctoral Science Foundation (Grant No. ZJ2023111) for supporting this research.
- Thanks to Ningbo Zhongchun GaoKe Co., Ltd. for providing the test site.
