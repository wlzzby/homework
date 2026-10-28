# Homework 2 — Atmospheric Dynamics
# 大气动力学作业二

本文件整理第 1.11–1.13 题，每题先给英文解答，再给中文解答。

This file covers Problems 1.11–1.13. Each problem is presented in English first and then in Chinese.

---

## Problem 1.11 — Motion of a frictionless particle initially moving northward

### English solution

Let $u$ and $v$ be the eastward and northward velocity components. For a frictionless particle moving horizontally at latitude $\phi$, the equations of motion are

$$
\frac{du}{dt}=fv,\qquad \frac{dv}{dt}=-fu,
\qquad f=2\Omega\sin\phi
$$

Initially, the particle moves northward with speed $V_0$, so

$$
u(0)=0,\qquad v(0)=V_0
$$

Differentiating the first equation and using the second gives

$$
\frac{d^2u}{dt^2}+f^2u=0
$$

Applying the initial conditions yields

$$
u(t)=V_0\sin ft,\qquad v(t)=V_0\cos ft
$$

With $dx/dt=u$ and $dy/dt=v$, and $x(0)=y(0)=0$,

$$
x(t)=\frac{V_0}{f}(1-\cos ft),\qquad
y(t)=\frac{V_0}{f}\sin ft
$$

These equations describe a circle:

$$
\left(x-\frac{V_0}{f}\right)^2+y^2
=\left(\frac{V_0}{f}\right)^2
$$

The radius is $V_0/|f|$. In the Northern Hemisphere, the trajectory curves to the right of the motion and is clockwise in the $x$-east, $y$-north coordinate plane. In the Southern Hemisphere, the curvature is reversed. At the equator, $f=0$, so the idealized motion is a straight line northward.

### 中文解答

设 $u$、$v$ 分别为向东和向北的速度分量。忽略摩擦时，位于纬度 $\phi$ 的水平运动满足

$$
\frac{du}{dt}=fv,\qquad \frac{dv}{dt}=-fu,
\qquad f=2\Omega\sin\phi
$$

初始时质点以速度 $V_0$ 向北运动，因此

$$
u(0)=0,\qquad v(0)=V_0
$$

对第一个方程求导，并代入第二个方程：

$$
\frac{d^2u}{dt^2}+f^2u=0
$$

结合初始条件，得到

$$
u(t)=V_0\sin ft,\qquad v(t)=V_0\cos ft
$$

由 $dx/dt=u$、$dy/dt=v$，并取 $x(0)=y(0)=0$，积分可得

$$
x(t)=\frac{V_0}{f}(1-\cos ft),\qquad
y(t)=\frac{V_0}{f}\sin ft
$$

轨迹满足

$$
\left(x-\frac{V_0}{f}\right)^2+y^2
=\left(\frac{V_0}{f}\right)^2
$$

因此为圆周运动，半径为 $V_0/|f|$。北半球中，运动轨迹向运动方向的右侧弯曲；在以东为 $x$、以北为 $y$ 的坐标平面中，轨迹为顺时针方向。南半球的弯曲方向相反。赤道上 $f=0$，在该理想化条件下质点沿初始方向作直线运动。


### Derivation details / 推导补充

**English.** Differentiate $du/dt=fv$ with respect to time. For constant latitude, $f$ is constant, so $d^2u/dt^2=f(dv/dt)=-f^2u$. Thus $u$ satisfies a simple harmonic oscillator equation. Its general solution is $u=A\sin ft+B\cos ft$. The initial condition $u(0)=0$ gives $B=0$, and $du/dt|_{t=0}=fV_0$ gives $Af=fV_0$, so $A=V_0$. Substituting into $dv/dt=-fu$ and applying $v(0)=V_0$ gives $v=V_0\cos ft$. Integrating the two velocity components gives the stated position equations. The circle equation follows by rearranging $x-V_0/f=-(V_0/f)\cos ft$ and $y=(V_0/f)\sin ft$, then using $\sin^2ft+\cos^2ft=1$.

**中文。** 对 $du/dt=fv$ 再对时间求导。固定纬度下 $f$ 为常数，因此 $d^2u/dt^2=f(dv/dt)=-f^2u$，从而得到简谐振动方程。其通解为 $u=A\sin ft+B\cos ft$。由 $u(0)=0$ 得 $B=0$；又因为初始时 $du/dt=fV_0$，所以 $Af=fV_0$，即 $A=V_0$。再将 $u$ 代入 $dv/dt=-fu$，并利用 $v(0)=V_0$，得到 $v=V_0\cos ft$。分别对两个速度分量积分即可得到位置方程。将位置方程改写为 $x-V_0/f=-(V_0/f)\cos ft$ 和 $y=(V_0/f)\sin ft$，两式平方相加并利用 $\sin^2ft+\cos^2ft=1$，便可证明轨迹为圆。

---

## Problem 1.12 — Thickness of an isothermal 1000–500 hPa layer

### English solution

For a hydrostatic atmosphere, the hypsometric equation is

$$
Z_2-Z_1=\frac{R_d\overline{T}}{g}
\ln\left(\frac{p_1}{p_2}\right)
$$

For an isothermal layer, $\overline{T}=T$. Between 1000 and 500 hPa,

$$
\Delta Z=\frac{R_dT}{g}\ln2
$$

Using $R_d=287\ {\rm J\,kg^{-1}\,K^{-1}}$ and $g=9.81\ {\rm m\,s^{-2}}$:

- For $T=273\ {\rm K}$,
  $

  \Delta Z\approx\frac{287(273)}{9.81}\ln2
  \approx5534\ {\rm m}.
  

$$
- For $T=250\ {\rm K}$,
  $

  \Delta Z\approx\frac{287(250)}{9.81}\ln2
  \approx5068\ {\rm m}
$$

The difference is approximately $5534-5068=466\ {\rm m}$. The warmer isothermal layer is thicker because the hypsometric thickness is proportional to mean absolute temperature.

### 中文解答

静力平衡条件下，测高公式为

$$
Z_2-Z_1=\frac{R_d\overline{T}}{g}
\ln\left(\frac{p_1}{p_2}\right)
$$

对于等温层，平均温度就是该层温度 $T$。在 1000–500 hPa 之间，

$$
\Delta Z=\frac{R_dT}{g}\ln2
$$

取 $R_d=287\ {\rm J\,kg^{-1}\,K^{-1}}$、$g=9.81\ {\rm m\,s^{-2}}$：

- 当 $T=273\ {\rm K}$ 时，
  $

  \Delta Z\approx\frac{287(273)}{9.81}\ln2
  \approx5534\ {\rm m}.
  

$$
- 当 $T=250\ {\rm K}$ 时，
  $

  \Delta Z\approx\frac{287(250)}{9.81}\ln2
  \approx5068\ {\rm m}
$$

两者厚度相差约 $5534-5068=466\ {\rm m}$。测高公式表明，气层厚度与平均绝对温度成正比，因此温度较高的等温层更厚。


### Derivation details / 推导补充

**English.** The hypsometric equation follows from hydrostatic balance, $dp/dz=-\rho g$, together with the ideal-gas law $\rho=p/(R_dT)$. Substituting gives $dz=-(R_dT/g)\,dp/p$. For an isothermal layer, $T$ is constant, so integration from the lower level $(p_1,Z_1)$ to the upper level $(p_2,Z_2)$ gives $Z_2-Z_1=(R_dT/g)\ln(p_1/p_2)$. Here $p_1/p_2=1000/500=2$, so the thickness is proportional to $T$. The difference can therefore also be calculated directly as $\Delta Z_{273}-\Delta Z_{250}=(R_d/g)(273-250)\ln2\approx466\ \mathrm{m}$.

**中文。** 测高公式可由静力平衡方程 $dp/dz=-\rho g$ 和理想气体状态方程 $\rho=p/(R_dT)$ 推出。代入后有 $dz=-(R_dT/g)\,dp/p$。等温层中 $T$ 为常数，从下层气压 $p_1$ 积分到上层气压 $p_2$，得到 $Z_2-Z_1=(R_dT/g)\ln(p_1/p_2)$。本题 $p_1/p_2=1000/500=2$，因此厚度与绝对温度成正比。也可以直接计算两种温度下的厚度差：$\Delta Z_{273}-\Delta Z_{250}=(R_d/g)(273-250)\ln2\approx466\ \mathrm{m}$。

---

## Problem 1.13 — Temperature difference corresponding to a 60 m thickness contour interval

### English solution

From the hypsometric equation,

$$
\Delta Z=\frac{R_d\overline{T}}{g}
\ln\left(\frac{p_1}{p_2}\right)
$$

For fixed pressure levels, a small change in layer thickness corresponds to a change in mean temperature:

$$
\delta(\Delta Z)=\frac{R_d}{g}
\ln\left(\frac{p_1}{p_2}\right)\delta\overline{T}
$$

For a 1000–500 hPa layer and a contour interval of $60\ {\rm m}$,

$$
\delta\overline{T}
=\frac{g(60\ {\rm m})}{R_d\ln2}
\approx\frac{9.81\times60}{287\ln2}
\approx2.96\ {\rm K}
$$

Thus, a 60 m thickness contour interval corresponds to a mean-temperature difference of approximately $3\ {\rm K}$, assuming the pressure levels are 1000 and 500 hPa.

### 中文解答

由测高公式，

$$
\Delta Z=\frac{R_d\overline{T}}{g}
\ln\left(\frac{p_1}{p_2}\right)
$$

在固定气压层之间，气层厚度的微小变化与平均温度变化满足

$$
\delta(\Delta Z)=\frac{R_d}{g}
\ln\left(\frac{p_1}{p_2}\right)\delta\overline{T}
$$

对于 1000–500 hPa 气层，若厚度等值线间隔为 $60\ {\rm m}$，则

$$
\delta\overline{T}
=\frac{g(60\ {\rm m})}{R_d\ln2}
\approx\frac{9.81\times60}{287\ln2}
\approx2.96\ {\rm K}
$$

因此，在气压层为 1000–500 hPa 的前提下，60 m 的厚度等值线间隔约对应 $3\ {\rm K}$ 的层平均温度差。


### Derivation details / 推导补充

**English.** For fixed pressure levels, $R_d$, $g$, and $\ln(p_1/p_2)$ are constants. Differentiating the hypsometric equation with respect to the layer-mean temperature therefore gives $\delta(\Delta Z)=(R_d/g)\ln(p_1/p_2)\,\delta\overline T$. Rearranging isolates the temperature difference: $\delta\overline T=g\,\delta(\Delta Z)/[R_d\ln(p_1/p_2)]$. Substituting $\delta(\Delta Z)=60\ \mathrm{m}$ and $p_1/p_2=2$ gives approximately $2.96\ \mathrm{K}$. A temperature interval in kelvin has the same numerical size as a temperature interval in degrees Celsius.

**中文。** 当上下气压层固定时，$R_d$、$g$ 和 $\ln(p_1/p_2)$ 都是常数。对测高公式按层平均温度求变化量，得到 $\delta(\Delta Z)=(R_d/g)\ln(p_1/p_2)\,\delta\overline T$。移项后可解出温度差：$\delta\overline T=g\,\delta(\Delta Z)/[R_d\ln(p_1/p_2)]$。代入 $\delta(\Delta Z)=60\ \mathrm{m}$ 以及 $p_1/p_2=2$，得到约 $2.96\ \mathrm{K}$。温差以开尔文或摄氏度表示时，数值相同。
