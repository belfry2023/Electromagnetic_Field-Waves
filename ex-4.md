### 解答：平面波从空气斜入射到理想导体（垂直极化）

给定条件：
- 区域1（空气）：本征阻抗 ${\eta_0 = 120\pi  \Omega \approx 377  \Omega}$
- 区域2（理想导体）：本征阻抗 ${\eta_2 = 0}$
- 入射角 ${\theta_i = 30^\circ}$
- 入射电场幅度 ${E_0 = 100  \text{V/m}}$（垂直极化，即电场垂直于入射平面）
- 假设入射平面为 ${xz}$ 平面，界面为 ${z=0}$，区域1 (${z < 0}$) 为空气，区域2 (${z > 0}$) 为理想导体。

#### (1) 求反射系数 ${\Gamma}$

对于垂直极化（TE 波或 s 极化）的平面波斜入射到理想导体表面，反射系数 ${\Gamma_\perp}$ 的公式为：
${
\Gamma_\perp = \frac{\eta_2 \cos \theta_i - \eta_1 \cos \theta_t}{\eta_2 \cos \theta_i + \eta_1 \cos \theta_t}
}$
其中 ${\theta_t}$ 为透射角。由于区域2 是理想导体，${\eta_2 = 0}$，代入得：
${
\Gamma_\perp = \frac{0 \cdot \cos \theta_i - \eta_1 \cos \theta_t}{0 \cdot \cos \theta_i + \eta_1 \cos \theta_t} = \frac{-\eta_1 \cos \theta_t}{\eta_1 \cos \theta_t} = -1
}$
因此，反射系数 ${\Gamma = -1}$。

${
\boxed{\Gamma = -1}
}$

#### (2) 写出空气中合成波 ${E}$ 的表达式

入射波为垂直极化，电场沿 ${y}$ 方向。入射波电场表达式为：
${
\vec{E}_i = \hat{y} E_0 e^{-j k_1 (x \sin \theta_i - z \cos \theta_i)}
}$
其中 ${k_1 = \omega \sqrt{\mu_0 \epsilon_0}}$ 为空气中波数（${\omega}$ 为角频率）。

反射系数 ${\Gamma = -1}$，反射波电场表达式为：
${
\vec{E}_r = \hat{y} \Gamma E_0 e^{-j k_1 (x \sin \theta_i + z \cos \theta_i)} = \hat{y} (-1) E_0 e^{-j k_1 (x \sin \theta_i + z \cos \theta_i)}
}$

空气中合成波电场 ${\vec{E} = \vec{E}_i + \vec{E}_r}$：
${
\vec{E} = \hat{y} E_0 \left[ e^{-j k_1 (x \sin \theta_i - z \cos \theta_i)} - e^{-j k_1 (x \sin \theta_i + z \cos \theta_i)} \right]
}$
简化表达式：
${
\vec{E} = \hat{y} E_0 e^{-j k_1 x \sin \theta_i} \left[ e^{j k_1 z \cos \theta_i} - e^{-j k_1 z \cos \theta_i} \right]
}$
利用恒等式 ${e^{j\phi} - e^{-j\phi} = 2j \sin \phi}$，其中 ${\phi = k_1 z \cos \theta_i}$：
${
\vec{E} = \hat{y} E_0 e^{-j k_1 x \sin \theta_i} \cdot 2j \sin(k_1 z \cos \theta_i)
}$
代入已知值 ${\theta_i = 30^\circ}$，${\sin \theta_i = \frac{1}{2}}$，${\cos \theta_i = \frac{\sqrt{3}}{2}}$，${E_0 = 100  \text{V/m}}$：
${
\vec{E} = \hat{y} \cdot 2j \cdot 100 \cdot \sin\left(k_1 z \cdot \frac{\sqrt{3}}{2}\right) e^{-j k_1 x \cdot \frac{1}{2}}
}$
因此，合成波电场表达式为：
${
\vec{E} = \hat{y} \cdot 200j \cdot \sin\left(\frac{\sqrt{3}}{2} k_1 z\right) e^{-j \frac{k_1 x}{2}}  \text{V/m}
}$

${
\boxed{\vec{E} = \hat{y} \cdot 200j \cdot \sin\left(\dfrac{\sqrt{3}}{2} k_1 z\right) \exp\left(-j \dfrac{k_1 x}{2}\right)  \text{V/m}}
}$

#### (3) 求导体表面感应电流密度 ${J_s}$

在理想导体表面（${z = 0}$），感应电流密度 ${\vec{J}_s}$ 由磁场切向分量给出：
${
\vec{J}_s = \hat{n} \times \vec{H}_1
}$
其中 ${\hat{n}}$ 为界面法向单位矢量，指向导体外部（即 ${\hat{n} = \hat{z}}$)，${\vec{H}_1}$ 为区域1（空气）中在 ${z = 0^-}$ 处的磁场。

首先求合成磁场 ${\vec{H}}$。由合成电场 ${\vec{E} = \hat{y} E_y}$，其中 ${E_y = 2j E_0 \sin(k_1 z \cos \theta_i) e^{-j k_1 x \sin \theta_i}}$，利用麦克斯韦方程 ${\nabla \times \vec{E} = -j \omega \mu_0 \vec{H}}$，得：
${
\vec{H} = \frac{j}{\omega \mu_0} \nabla \times \vec{E}
}$
计算旋度 ${\nabla \times \vec{E}}$：
${
\nabla \times \vec{E} = \begin{vmatrix}
\hat{x} & \hat{y} & \hat{z} \\
\frac{\partial}{\partial x} & \frac{\partial}{\partial y} & \frac{\partial}{\partial z} \\
0 & E_y & 0
\end{vmatrix} = -\hat{x} \frac{\partial E_y}{\partial z} + \hat{z} \frac{\partial E_y}{\partial x}
}$
代入 ${E_y = 2j E_0 \sin(\beta z) e^{-j \alpha x}}$，其中 ${\alpha = k_1 \sin \theta_i}$，${\beta = k_1 \cos \theta_i}$：
${
\frac{\partial E_y}{\partial z} = 2j E_0 \beta \cos(\beta z) e^{-j \alpha x}, \quad \frac{\partial E_y}{\partial x} = 2j E_0 \sin(\beta z) \cdot (-j \alpha) e^{-j \alpha x} = 2 \alpha E_0 \sin(\beta z) e^{-j \alpha x}
}$
所以：
${
\nabla \times \vec{E} = -\hat{x} \cdot 2j E_0 \beta \cos(\beta z) e^{-j \alpha x} + \hat{z} \cdot 2 \alpha E_0 \sin(\beta z) e^{-j \alpha x}
}$
代入 ${\vec{H}}$：
${
\vec{H} = \frac{j}{\omega \mu_0} \left[ -2j E_0 \beta \cos(\beta z) e^{-j \alpha x} \hat{x} + 2 \alpha E_0 \sin(\beta z) e^{-j \alpha x} \hat{z} \right] = \hat{x} \frac{2 E_0 \beta \cos(\beta z) e^{-j \alpha x}}{\omega \mu_0} + \hat{z} \frac{2 j \alpha E_0 \sin(\beta z) e^{-j \alpha x}}{\omega \mu_0}
}$
在表面 ${z = 0}$，${\cos(0) = 1}$，${\sin(0) = 0}$，所以：
${
\vec{H}_1 \big|_{z=0^-} = \hat{x} \frac{2 E_0 \beta \cdot 1 \cdot e^{-j \alpha x}}{\omega \mu_0} + \hat{z} \cdot 0 = \hat{x} \frac{2 E_0 \beta}{\omega \mu_0} e^{-j \alpha x}
}$
代入 ${\beta = k_1 \cos \theta_i}$，${\alpha = k_1 \sin \theta_i}$，并利用 ${\omega \mu_0 = k_1 \eta_0}$（因为 ${\eta_0 = \sqrt{\mu_0 / \epsilon_0}}$，${k_1 = \omega \sqrt{\mu_0 \epsilon_0}}$)：
${
\vec{H}_1 \big|_{z=0^-} = \hat{x} \frac{2 E_0 (k_1 \cos \theta_i)}{k_1 \eta_0} e^{-j k_1 x \sin \theta_i} = \hat{x} \frac{2 E_0 \cos \theta_i}{\eta_0} e^{-j k_1 x \sin \theta_i}
}$
切向磁场为 ${\hat{x}}$ 分量。

现在计算 ${\vec{J}_s}$：
${
\vec{J}_s = \hat{n} \times \vec{H}_1 \big|_{z=0^-} = \hat{z} \times \left( \hat{x} \frac{2 E_0 \cos \theta_i}{\eta_0} e^{-j k_1 x \sin \theta_i} \right) = (\hat{z} \times \hat{x}) \frac{2 E_0 \cos \theta_i}{\eta_0} e^{-j k_1 x \sin \theta_i} = (-\hat{y}) \frac{2 E_0 \cos \theta_i}{\eta_0} e^{-j k_1 x \sin \theta_i}
}$
代入已知值 ${\theta_i = 30^\circ}$，${\cos \theta_i = \frac{\sqrt{3}}{2}}$，${\sin \theta_i = \frac{1}{2}}$，${E_0 = 100  \text{V/m}}$，${\eta_0 = 120\pi  \Omega}$：
${
\vec{J}_s = -\hat{y} \frac{2 \times 100 \times \frac{\sqrt{3}}{2}}{120\pi} e^{-j k_1 x \cdot \frac{1}{2}} = -\hat{y} \frac{100 \sqrt{3}}{120\pi} e^{-j \frac{k_1 x}{2}}
}$
简化系数：
${
\frac{100 \sqrt{3}}{120\pi} = \frac{5 \sqrt{3}}{6\pi}
}$
因此：
${
\vec{J}_s = -\hat{y} \frac{5 \sqrt{3}}{6\pi} e^{-j \frac{k_1 x}{2}}  \text{A/m}
}$

${
\boxed{\vec{J}_s = -\hat{y} \dfrac{5 \sqrt{3}}{6\pi} \exp\left(-j \dfrac{k_1 x}{2}\right)  \text{A/m}}
}$