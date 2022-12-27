# Structural similarity

## 1. Introduce
- SSIM(structural similarity index measure) is a method for predicting the perceived quality of digital television and cinematic pictures, as well as other kinds of digital images and videos. 
</br>

## 2. Algorithm
- ## SSIM(x, y) = $\frac {(2μ_{x}+C_{1})(2σ_{xy} + C_2)}{(μ^2_{x}+μ^2_{y}+C_1)(σ^2_{x}+σ^2_{y}+C_2)}$
    - $\mu _{x}$ the pixel sample mean of ${\displaystyle x}$ 
    - $\mu _{y}$ the pixel sample mean of ${\displaystyle y}$
    - ${\displaystyle \sigma _{x}^{2}}$ the variance of ${\displaystyle x}$
    - ${\displaystyle \sigma _{y}^{2}}$ the variance of ${\displaystyle y}$
    - ${\displaystyle \sigma _{xy}}$ the covariance of ${\displaystyle x}$ and ${\displaystyle y}$
    - ${\displaystyle c_{1}=(k_{1}L)^{2}}$, ${\displaystyle c_{2}=(k_{2}L)^{2}}$ two variables to stabilize the division with weak denominator
    - ${\displaystyle L}$ the dynamic range of the pixel-values (typically this is ${\displaystyle 2^{\ bits\ per\ pixel}-1}$
    - ${\displaystyle k_{1}=0.01}$ and ${\displaystyle k_{2}=0.03}$ by default

## 3. Reference 
- https://www.imatest.com/docs/ssim/
- https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=5596999