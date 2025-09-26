# Mitigating Instability in High Residual Adaptive Sampling for PINNs via Langevin Dynamics [Neurips 2025 Spotlight]
<div align="center">

**Minseok Jeong<sup>*,†</sup>**, **Giup Seo<sup>*</sup>**, and **Euiseok Hwang<sup>‡</sup>**  
(<sup>*</sup>Equal contribution, <sup>†</sup> Work done while at GIST. Now at KAIST, ACS, <sup>‡</sup>Corresponding author)

Electrical Engineering and Computer Science  
Gwangju Institute of Science and Technology (GIST)

<dsa950115@kaist.ac.kr>,  <guseo1120@gm.gist.ac.kr>,  <euiseokh@gist.ac.kr>
</div>

<div align="center">
  
![PINN_scheme_1](https://github.com/user-attachments/assets/fbc8e932-5182-4971-b1f8-7fff99ff7ab2)

</div>

### abstract 
Recently, physics-informed neural networks (PINNs) have gained attention in the scientific community for their potential to solve partial differential equations (PDEs). 
However, they face challenges related to resource efficiency and slow convergence. 
Adaptive sampling methods, which prioritize collocation points with high residuals, improve both efficiency and accuracy.
However, these methods often neglect points with medium or low residuals, which can affect stability as the complexity of the model increases. 
In this paper, we investigate this limitation and show that high residual-based approaches require stricter learning rate bounds to ensure stability. 
To address this, we propose a Langevin dynamics-based Adaptive Sampling (LAS) framework that is robust to various learning rates and model complexities. 
Our experiments demonstrate that the proposed method outperforms existing approaches in terms of relative $L^{2}$ error, and stability across a range of enviroments, including high-dimensional PDEs where Monte Carlo integration-based methods typically suffer from instability.
