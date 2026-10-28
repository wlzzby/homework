# Homework 1 — Atmospheric Dynamics
# 大气动力学作业一

本文件按“English solution → 中文解答”的顺序整理第 1.1、1.2 题。数值为近似值，采用地球标准参数。

This file presents Problems 1.1 and 1.2 in English first, followed by Chinese explanations. Numerical values are approximate and use standard Earth parameters.

---

## Problem 1.1 — Angle between gravitational force and effective gravity

### English solution

At latitude $\phi$, the gravitational acceleration points toward Earth's center, whereas the effective gravity is the vector sum of gravitational acceleration and centrifugal acceleration. The centrifugal acceleration has magnitude $\Omega^2 R\cos\phi$, where $\Omega$ is Earth's angular velocity and $R$ is Earth's radius.

Resolve the accelerations into the radial and northward directions. Let

$$
\epsilon=\frac{\Omega^2R^3}{GM}
$$

where $GM/R^2$ is the magnitude of gravitational acceleration in the spherical-Earth approximation. The centrifugal components are

$$
a_{c,r}=\Omega^2R\cos^2\phi,\qquad
a_{c,n}=-\Omega^2R\sin\phi\cos\phi
$$

The effective-gravity components are therefore

$$
g_{e,r}=-\frac{GM}{R^2}+\Omega^2R\cos^2\phi,
\qquad
g_{e,n}=-\Omega^2R\sin\phi\cos\phi
$$

The angle $\theta$ between gravitational acceleration and effective gravity satisfies

$$
\tan\theta=
\frac{\Omega^2R|\sin\phi\cos\phi|}
{GM/R^2-\Omega^2R\cos^2\phi}
=\frac{\epsilon|\sin\phi\cos\phi|}
{1-\epsilon\cos^2\phi}
$$

For Earth's small parameter $\epsilon\approx 0.00346$, the small-angle approximation gives

$$
\theta\approx \epsilon|\sin\phi\cos\phi|
=\frac{\epsilon}{2}|\sin2\phi|
$$

The angle is zero at the equator and poles, and it is largest near $|\phi|=45^\circ$. The maximum is approximately

$$
\theta_{\max}\approx\frac{\epsilon}{2}
=0.00173\ {\rm rad}\approx0.099^\circ
$$

Thus, centrifugal acceleration causes effective gravity to deviate slightly from the direction toward Earth's center, with the largest deviation at mid-latitudes.

### 中文解答

在纬度 $\phi$ 处，万有引力加速度指向地心，而有效重力是万有引力加速度与地球自转产生的离心加速度的矢量和。离心加速度的大小为 $\Omega^2R\cos\phi$，其中 $\Omega$ 为地球自转角速度，$R$ 为地球半径。

将离心加速度分解为径向和向北分量。定义

$$
\epsilon=\frac{\Omega^2R^3}{GM}
$$

其中球形地球近似下万有引力加速度大小为 $GM/R^2$。离心加速度的分量为

$$
a_{c,r}=\Omega^2R\cos^2\phi,\qquad
a_{c,n}=-\Omega^2R\sin\phi\cos\phi
$$

因此，有效重力的分量为

$$
g_{e,r}=-\frac{GM}{R^2}+\Omega^2R\cos^2\phi,
\qquad
g_{e,n}=-\Omega^2R\sin\phi\cos\phi
$$

万有引力方向与有效重力方向的夹角 $\theta$ 满足

$$
\tan\theta=
\frac{\Omega^2R|\sin\phi\cos\phi|}
{GM/R^2-\Omega^2R\cos^2\phi}
=\frac{\epsilon|\sin\phi\cos\phi|}
{1-\epsilon\cos^2\phi}
$$

由于地球的 $\epsilon\approx0.00346$ 很小，可采用小角度近似：

$$
\theta\approx\epsilon|\sin\phi\cos\phi|
=\frac{\epsilon}{2}|\sin2\phi|
$$

在赤道和两极，夹角为零；在 $|\phi|\approx45^\circ$ 附近，夹角最大：

$$
\theta_{\max}\approx\frac{\epsilon}{2}
=0.00173\ {\rm rad}\approx0.099^\circ
$$

因此，离心加速度使有效重力方向略微偏离指向地心的方向，且这种偏离在中纬度附近最大。


### Derivation details / 推导补充

**English.** The gravitational acceleration has only a radial component, with magnitude $g=GM/R^2$. The centrifugal acceleration is directed away from Earth's rotation axis. At latitude $\phi$, its horizontal distance from the axis is $R\cos\phi$, so its magnitude is $\Omega^2R\cos\phi$. Resolving it gives a radial component $\Omega^2R\cos^2\phi$ and a northward component $-\Omega^2R\sin\phi\cos\phi$ under the chosen sign convention. The angle is therefore found from the ratio of the magnitude of the northward component to the inward radial component:
$$
\tan\theta=
\frac{\Omega^2R|\sin\phi\cos\phi|}
{GM/R^2-\Omega^2R\cos^2\phi}.
$$
Dividing numerator and denominator by $GM/R^2$ introduces the dimensionless parameter $\epsilon=\Omega^2R^3/(GM)$. Since $\epsilon\ll1$, the denominator is close to one and $\tan\theta\approx\theta$, giving $\theta\approx(\epsilon/2)|\sin2\phi|$. The factor $|\sin2\phi|$ reaches one at $|\phi|=45^\circ$, which explains the latitude of the maximum.

**中文。** 万有引力加速度只有径向分量，大小为 $GM/R^2$。离心加速度背离地球自转轴；纬度为 $\phi$ 处到自转轴的距离是 $R\cos\phi$，所以离心加速度大小为 $\Omega^2R\cos\phi$。将其分解后得到径向分量 $\Omega^2R\cos^2\phi$ 和按所选符号约定表示的向北分量 $-\Omega^2R\sin\phi\cos\phi$。因此，夹角可由向北分量的绝对值与有效重力径向分量之比求得。分子、分母同除以 $GM/R^2$，即可引入无量纲参数 $\epsilon=\Omega^2R^3/(GM)$。由于 $\epsilon\ll1$，分母近似为 1，且小角度下 $\tan\theta\approx\theta$，于是得到 $\theta\approx(\epsilon/2)|\sin2\phi|$。当 $|\phi|=45^\circ$ 时，$|\sin2\phi|=1$，故夹角在该纬度附近最大。

---

## Problem 1.2 — Altitude of a synchronous equatorial satellite

### English solution

A satellite in a circular equatorial orbit is synchronous when its angular velocity equals Earth's rotation rate $\Omega$. Equating gravitational acceleration to the required centripetal acceleration,

$$
\frac{GM}{r^2}=\Omega^2r
$$

where $r$ is the distance from the satellite to Earth's center. Hence,

$$
r=\left(\frac{GM}{\Omega^2}\right)^{1/3}
$$

Using $GM\approx3.986\times10^{14}\ {\rm m^3\,s^{-2}}$ and the sidereal rotation period $T\approx86164\ {\rm s}$, with $\Omega=2\pi/T$, gives

$$
r\approx4.216\times10^7\ {\rm m}
$$

Taking Earth's mean radius as $R_E\approx6.371\times10^6\ {\rm m}$, the altitude above the surface is

$$
h=r-R_E\approx3.579\times10^7\ {\rm m}
\approx35\,800\ {\rm km}
$$

The orbital period is one sidereal day, and the satellite remains above approximately the same point on the equator.

### 中文解答

赤道上的圆轨道卫星若要相对于地面保持静止，其角速度必须等于地球自转角速度 $\Omega$。令万有引力提供向心加速度：

$$
\frac{GM}{r^2}=\Omega^2r
$$

其中 $r$ 是卫星到地心的距离。解得

$$
r=\left(\frac{GM}{\Omega^2}\right)^{1/3}
$$

取 $GM\approx3.986\times10^{14}\ {\rm m^3\,s^{-2}}$，恒星日 $T\approx86164\ {\rm s}$，并令 $\Omega=2\pi/T$，可得

$$
r\approx4.216\times10^7\ {\rm m}
$$

取地球平均半径 $R_E\approx6.371\times10^6\ {\rm m}$，卫星离地高度为

$$
h=r-R_E\approx3.579\times10^7\ {\rm m}
\approx35\,800\ {\rm km}
$$

因此，同步卫星的轨道周期为一个恒星日；当轨道位于赤道平面且为顺行圆轨道时，卫星可相对地面保持在近似固定的经度上。


### Derivation details / 推导补充

**English.** Synchronous motion requires the satellite to have the same angular velocity as Earth, so its orbital period is one sidereal day. For a circular orbit, the required centripetal acceleration is $\Omega^2r$, while gravity provides $GM/r^2$. Equating them gives $GM/r^2=\Omega^2r$, or $r^3=GM/\Omega^2$. Taking the cube root yields the orbital radius measured from Earth's center. The requested altitude is not $r$ itself: Earth's radius must be subtracted, $h=r-R_E$. Using a sidereal day rather than a 24-hour solar day is important because the satellite must match Earth's rotation relative to the stars.

**中文。** 同步轨道要求卫星角速度与地球自转角速度相同，因此轨道周期为一个恒星日。圆周运动所需的向心加速度为 $\Omega^2r$，由万有引力提供的加速度为 $GM/r^2$。令二者相等，得到 $GM/r^2=\Omega^2r$，即 $r^3=GM/\Omega^2$，开立方即可得到以地心为基准的轨道半径。题目要求的是离地高度，而不是地心距，因此还需减去地球平均半径：$h=r-R_E$。这里应采用恒星日而非平均太阳日，因为卫星需要与地球相对于恒星的自转保持同步。
