# Homework 3 — Atmospheric Dynamics
# 大气动力学作业三

本文件整理第 2.6–2.8 题，每题先给英文解答，再给中文解答。

This file covers Problems 2.6–2.8. Each solution is given in English first and then in Chinese.

---

## Problem 2.6 — Density after adiabatic expansion

### English solution

For a dry ideal gas undergoing a reversible adiabatic process, Poisson's relation can be written as

$$

\frac{p}{\rho^\gamma}=\text{constant}

$$

where $\gamma=c_p/c_v\approx1.4$ for dry air. Between the initial state $(p_s,\rho_s)$ and the final state $(p,\rho)$,

$$

\frac{p_s}{\rho_s^\gamma}=\frac{p}{\rho^\gamma}

$$

Rearranging gives

$$

\rho^\gamma=\rho_s^\gamma\frac{p}{p_s},
\qquad
\boxed{\rho=\rho_s\left(\frac{p}{p_s}\right)^{1/\gamma}}

$$

For dry air, $1/\gamma\approx0.714\approx5/7$. Since $p<p_s$ during expansion, the density decreases. This expression assumes an ideal gas and a dry adiabatic process with no heat exchange.

### 中文解答

干燥理想气体经历可逆绝热过程时，泊松关系可写为

$$

\frac{p}{\rho^\gamma}=\text{常数}

$$

其中 $\gamma=c_p/c_v$，对干空气可近似取 $\gamma\approx1.4$。由初态 $(p_s,\rho_s)$ 到末态 $(p,\rho)$，有

$$

\frac{p_s}{\rho_s^\gamma}=\frac{p}{\rho^\gamma}

$$

整理得到

$$

\rho^\gamma=\rho_s^\gamma\frac{p}{p_s},
\qquad
\boxed{\rho=\rho_s\left(\frac{p}{p_s}\right)^{1/\gamma}}

$$

对干空气，$1/\gamma\approx0.714\approx5/7$。绝热膨胀时 $p<p_s$，因此密度随之减小。该结果适用于理想气体的干绝热过程，并假设没有热量交换。

---

## Problem 2.7 — A parcel lifted dry adiabatically from 1000 to 500 hPa

### English solution

The parcel initially has temperature

$$

T_s=20^\circ{\rm C}=293.15\ {\rm K}

$$

at $p_s=1000\ {\rm hPa}$, and is lifted dry adiabatically to $p=500\ {\rm hPa}$.

The dry-adiabatic temperature relation is

$$

T=T_s\left(\frac{p}{p_s}\right)^{R_d/c_p}

$$

where $R_d/c_p\approx0.286$. Therefore,

$$

T=293.15(0.5)^{0.286}\approx240.3\ {\rm K}

$$

(about $-32.9^\circ{\rm C}$).

The density at the initial state follows from the ideal-gas law:

$$

\rho_s=\frac{p_s}{R_dT_s}
=\frac{100000}{287(293.15)}
\approx1.188\ {\rm kg\,m^{-3}}

$$

Using the density relation from Problem 2.6,

$$

\rho=\rho_s\left(\frac{p}{p_s}\right)^{1/\gamma}
=1.188(0.5)^{1/1.4}
\approx0.724\ {\rm kg\,m^{-3}}

$$

Thus, the final density is approximately $0.72\ {\rm kg\,m^{-3}}$. The calculation neglects moisture and assumes the parcel remains unsaturated.

### 中文解答

气块初始温度为

$$

T_s=20^\circ{\rm C}=293.15\ {\rm K}

$$

初始气压 $p_s=1000\ {\rm hPa}$，随后沿干绝热过程上升至 $p=500\ {\rm hPa}$。

干绝热温度关系为

$$

T=T_s\left(\frac{p}{p_s}\right)^{R_d/c_p}

$$

其中 $R_d/c_p\approx0.286$。因此，

$$

T=293.15(0.5)^{0.286}\approx240.3\ {\rm K}

$$

约为 $-32.9^\circ{\rm C}$。

由理想气体状态方程，初始密度为

$$

\rho_s=\frac{p_s}{R_dT_s}
=\frac{100000}{287(293.15)}
\approx1.188\ {\rm kg\,m^{-3}}

$$

再利用第 2.6 题的密度关系：

$$

\rho=\rho_s\left(\frac{p}{p_s}\right)^{1/\gamma}
=1.188(0.5)^{1/1.4}
\approx0.724\ {\rm kg\,m^{-3}}

$$

因此，气块上升到 500 hPa 后的密度约为 $0.72\ {\rm kg\,m^{-3}}$。计算忽略水汽影响，并假设气块始终未达到饱和。

---

## Problem 2.8 — Buoyant acceleration and vertical speed of a warm parcel

### English solution

A parcel begins at rest at 800 hPa and is 1 K warmer than its environment as it rises to 500 hPa. Assume the layer-mean environmental temperature is $T=260\ {\rm K}$, the temperature excess $\Delta T=1\ {\rm K}$ is representative of the layer, and pressure remains close enough between parcel and environment that the ideal-gas approximation gives

$$

\frac{\rho_p-\rho_e}{\rho_e}\approx-\frac{\Delta T}{T}

$$

The buoyancy acceleration is

$$

B=-g\frac{\rho_p-\rho_e}{\rho_e}
\approx g\frac{\Delta T}{T}
=\frac{9.81}{260}
\approx0.0377\ {\rm m\,s^{-2}}

$$

Estimate the layer thickness using the hypsometric equation:

$$

\Delta z=\frac{R_dT}{g}\ln\left(\frac{800}{500}\right)
=\frac{287(260)}{9.81}\ln(1.6)
\approx3580\ {\rm m}

$$

If the buoyancy is approximately constant, the work per unit mass is

$$

W\approx B\Delta z
\approx0.0377(3580)\approx135\ {\rm J\,kg^{-1}}

$$

Starting from rest and neglecting drag and other forces, the kinetic-energy relation gives

$$

\frac{w^2}{2}=W,\qquad
w\approx\sqrt{2W}\approx16.4\ {\rm m\,s^{-1}}

$$

This is an idealized estimate; entrainment, pressure perturbations, and variation of buoyancy with height would modify the actual vertical speed.

### 中文解答

气块在 800 hPa 处由静止开始上升，在上升至 500 hPa 的过程中比环境高 $1\ {\rm K}$。设该层环境平均温度为 $T=260\ {\rm K}$，并近似认为温差 $\Delta T=1\ {\rm K}$ 在整个气层内具有代表性。若气块与环境气压近似相同，由理想气体状态方程可得

$$

\frac{\rho_p-\rho_e}{\rho_e}\approx-\frac{\Delta T}{T}

$$

浮力加速度为

$$

B=-g\frac{\rho_p-\rho_e}{\rho_e}
\approx g\frac{\Delta T}{T}
=\frac{9.81}{260}
\approx0.0377\ {\rm m\,s^{-2}}

$$

利用测高公式估算 800–500 hPa 气层厚度：

$$

\Delta z=\frac{R_dT}{g}\ln\left(\frac{800}{500}\right)
=\frac{287(260)}{9.81}\ln(1.6)
\approx3580\ {\rm m}

$$

若认为浮力在该层内近似不变，则单位质量气块受到浮力所做的功为

$$

W\approx B\Delta z
\approx0.0377(3580)\approx135\ {\rm J\,kg^{-1}}

$$

气块初始静止，忽略阻力及其他力的影响，由动能关系

$$

\frac{w^2}{2}=W,\qquad
w\approx\sqrt{2W}\approx16.4\ {\rm m\,s^{-1}}

$$

因此，估算的垂直速度约为 $16.4\ {\rm m\,s^{-1}}$。这是理想化估算；实际垂直速度还会受到卷入、压力扰动以及浮力随高度变化等因素影响。
