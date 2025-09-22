# Mitigating Instability in High Residual Adaptive Sampling for PINNs via Langevin Dynamics [Neurips 2025 Spotlight]
<div align="center">

**Minseok Jeong<sup>1,*</sup>**, **Giup Seo<sup>2,*</sup>**, and **Euiseok Hwang<sup>2</sup>**  (<sup>*</sup>Equal contribution  )

<sup>1</sup> KAIST, ACSS Lab  <sup>2</sup> GIST, IISL Lab  

</div>

<p align="center">
  <img src="https://github.com/user-attachments/assets/9a1a596d-2c21-4fd8-a9d2-d74e11cf5500" alt="PINN_scheme_1" width="500"/>
</p>

### abstract 
Recently, physics-informed neural networks (PINNs) have gained attention in the scientific community for their potential to solve partial differential equations (PDEs). 
However, they face challenges related to resource efficiency and slow convergence. 
Adaptive sampling methods, which prioritize collocation points with high residuals, improve both efficiency and accuracy.
However, these methods often neglect points with medium or low residuals, which can affect stability as the complexity of the model increases. 
In this paper, we investigate this limitation and show that high residual-based approaches require stricter learning rate bounds to ensure stability. 
To address this, we propose a Langevin dynamics-based Adaptive Sampling (LAS) framework that is robust to various learning rates and model complexities. 
Our experiments demonstrate that the proposed method outperforms existing approaches in terms of relative $L^{2}$ error, and stability across a range of enviroments, including high-dimensional PDEs where Monte Carlo integration-based methods typically suffer from instability.
