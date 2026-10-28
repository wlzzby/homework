# Homework 4 — Atmospheric Dynamics
# 大气动力学作业四

本文件整理第 3.10–3.12 题，每题先给英文解答，再给中文解答。涉及热成风的部分均采用北半球地转风和静力平衡近似。

This file covers Problems 3.10–3.12, with English solutions followed by Chinese solutions. The thermal-wind calculations use the Northern Hemisphere geostrophic and hydrostatic approximations.

---

## Problem 3.10 — Wind at 500 hPa from temperature gradient and 750 hPa wind

### English solution

The layer-mean temperature decreases eastward by $3^\circ{\rm C}$ per 100 km:
$

\frac{\partial\overline T}{\partial x}
=-\frac{3}{100000}
=-3.0\times10^{-5}\ {\rm K\,m^{-1}}.

$
Assume no meridional temperature gradient, so $\partial\overline T/\partial y=0$. The pressure-coordinate thermal-wind relations are
$

\frac{\partial u_g}{\partial\ln p}
=\frac{R_d}{f}\frac{\partial T}{\partial y},
\qquad
\frac{\partial v_g}{\partial\ln p}
=-\frac{R_d}{f}\frac{\partial T}{\partial x}.

$
Integrating from 750 to 500 hPa,
$

u_{500}-u_{750}
=\frac{R_d}{f}\frac{\partial\overline T}{\partial y}
\ln\left(\frac{500}{750}\right)=0,

$
and
$

v_{500}-v_{750}
=-\frac{R_d}{f}\frac{\partial\overline T}{\partial x}
\ln\left(\frac{500}{750}\right).

$
At the stated latitude, take $f=10^{-4}\ {\rm s^{-1}}$. Then
$

v_{500}-v_{750}
=-\frac{287}{10^{-4}}(-3.0\times10^{-5})
\ln(2/3)\approx-34.9\ {\rm m\,s^{-1}}.

$
A southeasterly wind at 750 hPa with speed $20\ {\rm m\,s^{-1}}$ has components
$

u_{750}=-20\sin45^\circ\approx-14.14\ {\rm m\,s^{-1}},
\quad
v_{750}=20\cos45^\circ\approx14.14\ {\rm m\,s^{-1}}.

$
Thus,
$

u_{500}\approx-14.14\ {\rm m\,s^{-1}},\qquad
v_{500}\approx-20.8\ {\rm m\,s^{-1}}.

$
The wind speed is
$

V_{500}=\sqrt{u_{500}^2+v_{500}^2}\approx25.2\ {\rm m\,s^{-1}}.

$
The vector points toward the southwest; meteorologically, the wind comes from the northeast, with a direction of approximately $034^\circ$ measured clockwise from north. This result follows from the stated eastward temperature decrease and the sign convention in the thermal-wind relation.

### 中文解答

气层平均温度向东每 100 km 降低 $3^\circ{\rm C}$，因此
$

\frac{\partial\overline T}{\partial x}
=-\frac{3}{100000}
=-3.0\times10^{-5}\ {\rm K\,m^{-1}}.

$
题目假设南北向温度梯度为零，即 $\partial\overline T/\partial y=0$。气压坐标下的热成风关系为
$

\frac{\partial u_g}{\partial\ln p}
=\frac{R_d}{f}\frac{\partial T}{\partial y},
\qquad
\frac{\partial v_g}{\partial\ln p}
=-\frac{R_d}{f}\frac{\partial T}{\partial x}.

$
从 750 hPa 积分到 500 hPa：
$

u_{500}-u_{750}
=\frac{R_d}{f}\frac{\partial\overline T}{\partial y}
\ln\left(\frac{500}{750}\right)=0,

$
$

v_{500}-v_{750}
=-\frac{R_d}{f}\frac{\partial\overline T}{\partial x}
\ln\left(\frac{500}{750}\right).

$
取 $f=10^{-4}\ {\rm s^{-1}}$，则
$

v_{500}-v_{750}
=-\frac{287}{10^{-4}}(-3.0\times10^{-5})
\ln(2/3)\approx-34.9\ {\rm m\,s^{-1}}.

$
750 hPa 的东南风风速为 $20\ {\rm m\,s^{-1}}$，其分量为
$

u_{750}=-20\sin45^\circ\approx-14.14\ {\rm m\,s^{-1}},
\quad
v_{750}=20\cos45^\circ\approx14.14\ {\rm m\,s^{-1}}.

$
因此，
$

u_{500}\approx-14.14\ {\rm m\,s^{-1}},\qquad
v_{500}\approx-20.8\ {\rm m\,s^{-1}}.

$
500 hPa 风速为
$

V_{500}=\sqrt{u_{500}^2+v_{500}^2}\approx25.2\ {\rm m\,s^{-1}}.

$
风矢量指向西南，因此按气象风向定义，风来自东北，风向约为从正北顺时针 $034^\circ$。该结果依赖于题设的向东降温条件及热成风关系中的符号约定。

---

## Problem 3.11 — Temperature advection by the layer-mean wind

### English solution

The horizontal temperature-advection rate is
$

-\mathbf V\cdot\nabla T
=-u\frac{\partial T}{\partial x}
-v\frac{\partial T}{\partial y}.

$
For the stated case, take the eastward temperature gradient as
$

\frac{\partial T}{\partial x}=-3.0\times10^{-5}\ {\rm K\,m^{-1}},

$
and the meridional gradient as zero. Using the layer-mean wind components $u= -14.14\ {\rm m\,s^{-1}}$ and $v=14.14\ {\rm m\,s^{-1}}$ (the southeasterly flow specified for the layer),
$

-\mathbf V\cdot\nabla T
=-u\frac{\partial T}{\partial x}
=-(-14.14)(-3.0\times10^{-5})
\approx-4.24\times10^{-4}\ {\rm K\,s^{-1}}.

$
Converting units,
$

-4.24\times10^{-4}\times3600
\approx-1.53\ {\rm K\,h^{-1}}.

$
The result is negative, indicating cold advection under the convention that a negative temperature tendency due to advection represents cooling. The numerical result depends on the wind components and temperature gradient specified in the problem.

### 中文解答

水平温度平流率为
$

-\mathbf V\cdot\nabla T
=-u\frac{\partial T}{\partial x}
-v\frac{\partial T}{\partial y}.

$
对本题，取向东温度梯度
$

\frac{\partial T}{\partial x}=-3.0\times10^{-5}\ {\rm K\,m^{-1}},

$
并假设南北向温度梯度为零。若采用题设气层的平均东向风分量 $u=-14.14\ {\rm m\,s^{-1}}$、北向风分量 $v=14.14\ {\rm m\,s^{-1}}$，则
$

-\mathbf V\cdot\nabla T
=-u\frac{\partial T}{\partial x}
=-(-14.14)(-3.0\times10^{-5})
\approx-4.24\times10^{-4}\ {\rm K\,s^{-1}}.

$
换算为每小时：
$

-4.24\times10^{-4}\times3600
\approx-1.53\ {\rm K\,h^{-1}}.

$
结果为负，表示温度平流导致降温，即冷平流。该数值取决于题目给定的风分量和温度梯度。

---

## Problem 3.12 — Thermal-wind temperature gradients and temperature advection

### English solution

At latitude $43^\circ{\rm N}$,
$

f=2\Omega\sin43^\circ\approx9.94\times10^{-5}\ {\rm s^{-1}}.

$
Use the pressure-coordinate thermal-wind relations
$

\frac{\partial u_g}{\partial\ln p}
=\frac{R_d}{f}\frac{\partial T}{\partial y},
\qquad
\frac{\partial v_g}{\partial\ln p}
=-\frac{R_d}{f}\frac{\partial T}{\partial x}.

$
For a layer bounded by pressures $p_b$ and $p_t$, approximate the vertical derivative by
$

\Delta u_g\approx\frac{R_d}{f}\frac{\partial\overline T}{\partial y}
\ln\left(\frac{p_t}{p_b}\right),\qquad
\Delta v_g\approx-\frac{R_d}{f}\frac{\partial\overline T}{\partial x}
\ln\left(\frac{p_t}{p_b}\right).

$

**Layer 900–700 hPa.** The 900 hPa wind is southerly at $10\ {\rm m\,s^{-1}}$, so $(u,v)_{900}=(0,10)$. The 700 hPa wind is westerly at $10\ {\rm m\,s^{-1}}$, so $(u,v)_{700}=(10,0)$. Therefore, $\Delta u=10$ and $\Delta v=-10\ {\rm m\,s^{-1}}$. Substitution gives approximately
$

\frac{\partial\overline T}{\partial y}
\approx-1.38\times10^{-5}\ {\rm K\,m^{-1}},\qquad
\frac{\partial\overline T}{\partial x}
\approx-1.38\times10^{-5}\ {\rm K\,m^{-1}}.

$

**Layer 700–500 hPa.** The 700 hPa wind is $(10,0)$ and the 500 hPa wind is $(20,0)\ {\rm m\,s^{-1}}$. Hence $\Delta u=10$ and $\Delta v=0$, giving approximately
$

\frac{\partial\overline T}{\partial y}
\approx-1.03\times10^{-5}\ {\rm K\,m^{-1}},\qquad
\frac{\partial\overline T}{\partial x}\approx0.

$

Estimate the mean wind in each layer by averaging the winds at its bounding levels. For 900–700 hPa,
$

(\bar u,\bar v)=(5,5)\ {\rm m\,s^{-1}}.

$
The temperature-advection rate is
$

-\bar u\frac{\partial\overline T}{\partial x}
-\bar v\frac{\partial\overline T}{\partial y}
\approx1.38\times10^{-4}\ {\rm K\,s^{-1}}
\approx0.50\ {\rm K\,h^{-1}},

$
which is warm advection. For 700–500 hPa, the mean wind is $(15,0)\ {\rm m\,s^{-1}}$ and the estimated zonal temperature gradient is zero, so the mean horizontal temperature advection is approximately zero.

Finally, the dry-adiabatic lapse rate is
$

\Gamma_d=\frac{g}{c_p}\approx9.78\ {\rm K\,km^{-1}}.

$
The 800–600 hPa layer thickness is approximately $2.25\ {\rm km}$ for a representative mean temperature near 260 K. The temperature difference associated with a dry-adiabatic lapse rate across this depth is
$

\Delta T_d\approx\Gamma_d\Delta z
\approx9.78(2.25)\approx22.0\ {\rm K}.

$
If the warm-advection rate of about $0.50\ {\rm K\,h^{-1}}$ is treated as constant and representative, a rough timescale is
$

t\approx\frac{22.0}{0.50}\approx44\ {\rm h}.

$
This final estimate is highly idealized: the actual time depends on the evolution of the flow and temperature gradients, vertical motion, and the precise interpretation of the question's stability criterion.

### 中文解答

在 $43^\circ{\rm N}$ 纬度处，
$

f=2\Omega\sin43^\circ\approx9.94\times10^{-5}\ {\rm s^{-1}}.

$
采用气压坐标下的热成风关系：
$

\frac{\partial u_g}{\partial\ln p}
=\frac{R_d}{f}\frac{\partial T}{\partial y},
\qquad
\frac{\partial v_g}{\partial\ln p}
=-\frac{R_d}{f}\frac{\partial T}{\partial x}.

$
对上下边界气压分别为 $p_b$、$p_t$ 的气层，可近似写为
$

\Delta u_g\approx\frac{R_d}{f}\frac{\partial\overline T}{\partial y}
\ln\left(\frac{p_t}{p_b}\right),\qquad
\Delta v_g\approx-\frac{R_d}{f}\frac{\partial\overline T}{\partial x}
\ln\left(\frac{p_t}{p_b}\right).

$

**900–700 hPa 气层。** 900 hPa 为风速 $10\ {\rm m\,s^{-1}}$ 的南风，因此 $(u,v)_{900}=(0,10)$；700 hPa 为风速 $10\ {\rm m\,s^{-1}}$ 的西风，因此 $(u,v)_{700}=(10,0)$。于是 $\Delta u=10$、$\Delta v=-10\ {\rm m\,s^{-1}}$。代入热成风关系得
$

\frac{\partial\overline T}{\partial y}
\approx-1.38\times10^{-5}\ {\rm K\,m^{-1}},\qquad
\frac{\partial\overline T}{\partial x}
\approx-1.38\times10^{-5}\ {\rm K\,m^{-1}}.

$

**700–500 hPa 气层。** 700 hPa 风分量为 $(10,0)$，500 hPa 风分量为 $(20,0)\ {\rm m\,s^{-1}}$，因此 $\Delta u=10$、$\Delta v=0$。相应温度梯度为
$

\frac{\partial\overline T}{\partial y}
\approx-1.03\times10^{-5}\ {\rm K\,m^{-1}},\qquad
\frac{\partial\overline T}{\partial x}\approx0.

$

用气层上下边界风的算术平均估计层平均风。对 900–700 hPa 气层，
$

(\bar u,\bar v)=(5,5)\ {\rm m\,s^{-1}}.

$
温度平流率为
$

-\bar u\frac{\partial\overline T}{\partial x}
-\bar v\frac{\partial\overline T}{\partial y}
\approx1.38\times10^{-4}\ {\rm K\,s^{-1}}
\approx0.50\ {\rm K\,h^{-1}},

$
对应暖平流。对 700–500 hPa 气层，平均风为 $(15,0)\ {\rm m\,s^{-1}}$，且估算的东西向温度梯度为零，因此平均水平温度平流近似为零。

最后，干绝热直减率为
$

\Gamma_d=\frac{g}{c_p}\approx9.78\ {\rm K\,km^{-1}}.

$
当代表性平均温度约为 260 K 时，800–600 hPa 气层厚度约为 $2.25\ {\rm km}$。该厚度对应的干绝热温差为
$

\Delta T_d\approx\Gamma_d\Delta z
\approx9.78(2.25)\approx22.0\ {\rm K}.

$
若将约 $0.50\ {\rm K\,h^{-1}}$ 的暖平流率视为恒定且具有代表性，则粗略时间尺度为
$

t\approx\frac{22.0}{0.50}\approx44\ {\rm h}.

$
这一时间估算较为理想化。真实时间取决于风场和温度梯度的演变、垂直运动，以及题目对稳定度判据的具体定义。
