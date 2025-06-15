### 电磁场与电磁波期末复习资料（按PPT大纲精编）

---

#### **一、矢量分析（核心基础）**
1. **标量场梯度**
   - 直角坐标系：$\nabla \phi = \frac{\partial \phi}{\partial x}\vec{e_x} + \frac{\partial \phi}{\partial y}\vec{e_y} + \frac{\partial \phi}{\partial z}\vec{e_z}$
   - 球坐标系：$\nabla \phi = \frac{\partial \phi}{\partial r}\vec{e_r} + \frac{1}{r}\frac{\partial \phi}{\partial \theta}\vec{e_\theta} + \frac{1}{r\sin\theta}\frac{\partial \phi}{\partial \phi}\vec{e_\phi}$
   - **物理意义**：方向为最大变化率，模为变化率最大值
2. **矢量场运算**
   - 散度（通量源）：
     - 直角系：$\nabla \cdot \vec{A} = \frac{\partial A_x}{\partial x} + \frac{\partial A_y}{\partial y} + \frac{\partial A_z}{\partial z}$
     - 球系：$\nabla \cdot \vec{A} = \frac{1}{r^2}\frac{\partial}{\partial r}(r^2A_r) + \frac{1}{r\sin\theta}\frac{\partial}{\partial \theta}(\sin\theta A_\theta) + \frac{1}{r\sin\theta}\frac{\partial A_\phi}{\partial \phi}$
   - 旋度（涡旋源）：
     - 直角系：$\nabla \times \vec{A} = \begin{vmatrix} \vec{e_x} & \vec{e_y} & \vec{e_z} \\ \frac{\partial}{\partial x} & \frac{\partial}{\partial y} & \frac{\partial}{\partial z} \\ A_x & A_y & A_z \end{vmatrix}$
3. **积分定理**
   - **高斯定理**：$\oint_S \vec{A} \cdot d\vec{s} = \int_V (\nabla \cdot \vec{A}) dv$
   - **斯托克斯定理**：$\oint_L \vec{A} \cdot d\vec{l} = \int_S (\nabla \times \vec{A}) \cdot d\vec{s}$

---

#### **二、静电场（重点章节）**
1. **基本方程**
   ```math
   \begin{cases}
   \nabla \times \vec{E} = 0 & \text{(无旋性)} \\
   \nabla \cdot \vec{D} = \rho & \text{(高斯定理)} \\
   \vec{D} = \epsilon \vec{E} & \text{(本构关系)}
   \end{cases}
   ```
2. **边界条件**
   - 电位移法向分量：$D_{1n} - D_{2n} = \sigma$（$\sigma$为自由电荷密度）
   - 电场切向分量：$E_{1t} = E_{2t}$
3. **电荷密度计算**
   - 自由电荷密度：$\rho = \nabla \cdot \vec{D}$
   - 极化电荷密度：$\rho_p = -\nabla \cdot \vec{P}$（$\vec{P}$为极化强度）
4. **电容计算**
   - 平行板电容：$C = \frac{\epsilon S}{d}$
   - 球形电容：$C = 4\pi\epsilon \frac{R_1 R_2}{R_2 - R_1}$

---

#### **三、恒定磁场（重点章节）**
1. **基本方程**
   ```math
   \begin{cases}
   \nabla \cdot \vec{B} = 0 & \text{(无散性)} \\
   \nabla \times \vec{H} = \vec{J} & \text{(安培定律)} \\
   \vec{B} = \mu_0(\vec{H} + \vec{M}) & \text{(磁介质)}
   \end{cases}
   ```
2. **矢量磁位**
   - $\vec{B} = \nabla \times \vec{A}$，库仑规范 $\nabla \cdot \vec{A} = 0$
   - 泊松方程：$\nabla^2 \vec{A} = -\mu \vec{J}$
3. **磁场能量**
   - 能量密度：$w_m = \frac{1}{2} \vec{B} \cdot \vec{H}$
   - 电感储能：$W_m = \frac{1}{2} L I^2$

---

#### **四、分离变量法与镜像法**
1. **直角坐标系分离变量**
   - 拉普拉斯方程：$\nabla^2 \phi = 0$
   - 通解形式：$\phi(x,y,z) = X(x)Y(y)Z(z)$
2. **镜像法应用**
   - 无限大导体平面：$q' = -q$（镜像对称位置）
   - 导体球：$q' = -\frac{a}{d}q$，$d' = \frac{a^2}{d}$（球心距）

---

#### **五、Poynting定理（能量守恒）**
- 瞬时Poynting矢量：$\vec{S} = \vec{E} \times \vec{H}$
- **平均功率密度**：$\vec{S}_{av} = \frac{1}{2} \text{Re}(\vec{E} \times \vec{H}^*)$
- 能量守恒：$-\frac{\partial}{\partial t} \int_V (w_e + w_m) dv = \oint_S \vec{S} \cdot d\vec{s} + \int_V \vec{J} \cdot \vec{E} dv$

---

#### **六、平面电磁波（重点章节）**
1. **波参数**
   - 波数：$k = \omega \sqrt{\mu \epsilon}$
   - 波阻抗：$\eta = \sqrt{\mu / \epsilon}$
   - 相速度：$v_p = \omega / \beta$
2. **反射与透射**
   - 垂直入射反射系数：$\Gamma = \frac{\eta_2 - \eta_1}{\eta_2 + \eta_1}$
   - 透射系数：$T = 1 + \Gamma$
   - 驻波比：$SWR = \frac{1 + |\Gamma|}{1 - |\Gamma|}$
3. **斜入射关键公式**
   - 折射定律：$\frac{\sin \theta_i}{\sin \theta_t} = \sqrt{\frac{\epsilon_2}{\epsilon_1}}$
   - 全反射临界角：$\theta_c = \arcsin\sqrt{\frac{\epsilon_2}{\epsilon_1}}$ ($\epsilon_1 > \epsilon_2$)

---

#### **七、天线基础**
- **电偶极子辐射**
  - 方向函数：$F(\theta) = \sin\theta$
  - 方向图：哑铃形三维辐射模式
- **基本参数**
  - 辐射功率：$P_r = \frac{I_m^2}{3} \pi \eta \left(\frac{dl}{\lambda}\right)^2$
  - 辐射电阻：$R_r = 80\pi^2 \left(\frac{dl}{\lambda}\right)^2$

---

### 重点公式速查表
| 概念                | 公式                                                                 |
|---------------------|----------------------------------------------------------------------|
| 电场高斯定理        | $\oint_S \vec{D} \cdot d\vec{s} = Q$                                |
| 磁场安培定律        | $\oint_L \vec{H} \cdot d\vec{l} = I$                                |
| 平面波波阻抗        | $\eta = \sqrt{\mu / \epsilon}$                                      |
| 临界角              | $\theta_c = \arcsin\sqrt{\epsilon_2 / \epsilon_1}$                  |

> **复习建议**：  
> 1. 矢量分析贯穿始终，务必熟练掌握三种坐标系转换  
> 2. 静电场/磁场重点练习边界条件应用（导体/介质界面）  
> 3. 平面波必考反射系数和极化计算  
> 4. 结合PDF中的推导过程理解镜像法原理  

祝考试顺利！ 💪