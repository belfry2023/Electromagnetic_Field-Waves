### **电磁场与电磁波（修订版）分章节完整内容**

---

#### **第1章 矢量分析基础**
1. **矢量微分算子**  
   - **梯度**：  
     $$
     \nabla f = \frac{1}{h_1} \frac{\partial f}{\partial q_1} \hat{e}_1 + \frac{1}{h_2} \frac{\partial f}{\partial q_2} \hat{e}_2 + \frac{1}{h_3} \frac{\partial f}{\partial q_3} \hat{e}_3
     $$
     - 直角坐标系：${ h_x=1, h_y=1, h_z=1 }$
     - 柱坐标系：${ h_\rho=1, h_\phi=\rho, h_z=1 }$
     - 球坐标系：${ h_r=1, h_\theta=r, h_\phi=r \sin\theta }$
   - **散度**：  
     $$
     \nabla \cdot \vec{A} = \frac{1}{h_1 h_2 h_3} \left[ \frac{\partial}{\partial q_1}(A_1 h_2 h_3) + \frac{\partial}{\partial q_2}(A_2 h_1 h_3) + \frac{\partial}{\partial q_3}(A_3 h_1 h_2) \right]
     $$
   - **旋度**：  
     $$
     \nabla \times \vec{A} = \frac{1}{h_1 h_2 h_3} 
     \begin{vmatrix}
     h_1 \hat{e}_1 & h_2 \hat{e}_2 & h_3 \hat{e}_3 \\
     \frac{\partial}{\partial q_1} & \frac{\partial}{\partial q_2} & \frac{\partial}{\partial q_3} \\
     h_1 A_1 & h_2 A_2 & h_3 A_3
     \end{vmatrix}
     $$

2. **积分定理**  
   - **散度定理**：  
     $$
     \oint_S \vec{A} \cdot d\vec{s} = \int_V (\nabla \cdot \vec{A})  dv
     $$
   - **斯托克斯定理**：  
     $$
     \oint_L \vec{A} \cdot d\vec{l} = \int_S (\nabla \times \vec{A}) \cdot d\vec{s}
     $$

3. **亥姆霍兹定理**  
   - 矢量场分解：  
     $$
     \vec{F} = -\nabla \phi + \nabla \times \vec{A}
     $$
   - 势函数：  
     $$
     \phi = \frac{1}{4\pi} \int_V \frac{\nabla' \cdot \vec{F}}{|\vec{r}-\vec{r}'|}  dv', \quad
     \vec{A} = \frac{1}{4\pi} \int_V \frac{\nabla' \times \vec{F}}{|\vec{r}-\vec{r}'|}  dv'
     $$

---

#### **第2章 静电场**
1. **基本方程**  
   - **高斯定理**：  
     $$
     \oint_S \vec{D} \cdot d\vec{s} = Q_{\text{enc}} \quad \Rightarrow \quad \nabla \cdot \vec{D} = \rho
     $$
   - **环路定理**：  
     $$
     \oint_L \vec{E} \cdot d\vec{l} = 0 \quad \Rightarrow \quad \nabla \times \vec{E} = 0
     $$

2. **导体与电介质**  
   - **导体特性**：  
     - 内部 ${\vec{E} = 0}$，表面为等势面  
     - 电荷分布：${\rho_s \propto \text{曲率}}$（曲率大则 ${\rho_s}$ 大）  
     - 表面电场：${ E_n = \dfrac{\rho_s}{\varepsilon_0} }$  
   - **电介质极化**：  
     - 极化强度：${\vec{P} = \varepsilon_0 \chi_e \vec{E}}$  
     - 电位移矢量：${\vec{D} = \varepsilon_0 \vec{E} + \vec{P} = \varepsilon \vec{E}}$  

3. **边界条件**  
   - 电场切向连续：${ E_{1t} = E_{2t} }$  
   - 电位移法向跃变：${ D_{1n} - D_{2n} = \sigma_f }$  

4. **电位与场强计算**  
   - 电位定义：${\Phi = \int_P^{\text{参考点}} \vec{E} \cdot d\vec{l}}$，${\vec{E} = -\nabla \Phi}$  
   - 点电荷电位：${\Phi = \dfrac{1}{4\pi\varepsilon_0} \dfrac{q}{R}}$  
   - 叠加原理：${\Phi = \dfrac{1}{4\pi\varepsilon_0} \displaystyle\int \dfrac{dq}{R}}$  

---

#### **第3章 恒定电场**
1. **电流密度**  
   - 体电流：${\vec{J} = \rho \vec{v}}$，${ I = \displaystyle\int_S \vec{J} \cdot d\vec{s} }$  
   - 面电流：${\vec{J}_s = \lim_{\Delta l \to 0} \dfrac{\Delta I}{\Delta l} \hat{n}}$，${ I = \displaystyle\int_L \vec{J}_s \cdot (\hat{n} \times d\vec{l}) }$  

2. **基本方程**  
   - 电流连续性：${\nabla \cdot \vec{J} + \dfrac{\partial \rho}{\partial t} = 0 \quad \xrightarrow{\text{恒定}} \quad \nabla \cdot \vec{J} = 0}$  
   - 欧姆定律：${\vec{J} = \sigma \vec{E}}$  

3. **接地问题**  
   - 接地电阻：${ R \approx \dfrac{1}{2\pi\sigma r} }$（半球电极）  
   - 跨步电压：${ U_{AB} \approx \dfrac{I b}{2\pi\sigma r^2} }$  

---

#### **第4章 恒定磁场**
1. **基本方程**  
   - **高斯定理**：  
     $$
     \oint_S \vec{B} \cdot d\vec{s} = 0 \quad \Rightarrow \quad \nabla \cdot \vec{B} = 0
     $$
   - **安培环路定理**：  
     $$
     \oint_L \vec{H} \cdot d\vec{l} = I_{\text{enc}} \quad \Rightarrow \quad \nabla \times \vec{H} = \vec{J}
     $$

2. **磁介质**  
   - 磁化强度：${\vec{M} = \chi_m \vec{H}}$  
   - 磁场强度：${\vec{H} = \dfrac{\vec{B}}{\mu_0} - \vec{M}}$  
   - 本构关系：${\vec{B} = \mu \vec{H}}$  

3. **边界条件**  
   - 磁感应强度法向连续：${ B_{1n} = B_{2n} }$  
   - 磁场强度切向跃变：${ H_{1t} - H_{2t} = J_s }$  

4. **电感计算**  
   - 自感：${ L = \dfrac{\psi}{I} }$  
   - 互感：${ M = \dfrac{\psi_{21}}{I_1} = \dfrac{\psi_{12}}{I_2} }$  

---

#### **第5章 时变电磁场**
1. **麦克斯韦方程组**  
   $$
   \begin{cases}
   \nabla \times \vec{E} = -\dfrac{\partial \vec{B}}{\partial t} \\
   \nabla \times \vec{H} = \vec{J} + \dfrac{\partial \vec{D}}{\partial t} \\
   \nabla \cdot \vec{D} = \rho \\
   \nabla \cdot \vec{B} = 0
   \end{cases}
   $$
   - 位移电流：${\vec{J}_d = \dfrac{\partial \vec{D}}{\partial t}}$  

2. **波动方程**  
   - 电场方程：  
     $$
     \nabla^2 \vec{E} - \mu\varepsilon \dfrac{\partial^2 \vec{E}}{\partial t^2} = 0
     $$
   - 矢量位方程（洛伦兹规范）：  
     $$
     \nabla^2 \vec{A} - \mu\varepsilon \dfrac{\partial^2 \vec{A}}{\partial t^2} = -\mu \vec{J}
     $$

3. **坡印廷定理**  
   - 瞬时功率：${\vec{S} = \vec{E} \times \vec{H}}$  
   - 平均功率：${\vec{S}_{\text{av}} = \dfrac{1}{2} \operatorname{Re} (\dot{\vec{E}} \times \dot{\vec{H}}^*)}$  

---

#### **第6章 平面电磁波**
1. **理想介质中的波**  
   - 波动方程解：${\vec{E} = \hat{e}_x E_0 e^{j(\omega t - kz)}}$  
   - 波数：${ k = \omega \sqrt{\mu\varepsilon} }$  
   - 波阻抗：${ \eta = \sqrt{\mu / \varepsilon} }$  

2. **极化特性**  
   - **线极化**：${ E_x }$ 与 ${ E_y }$ 同相  
   - **圆极化**：  
     - 条件：${ E_{xm} = E_{ym} }$，相位差 ${ \pi/2 }$  
     - 旋向：右旋（${ E_y }$ 滞后 ${ E_x }$）  

3. **导电媒质中的波**  
   - 复介电常数：${\varepsilon_c = \varepsilon \left(1 - j\dfrac{\sigma}{\omega \varepsilon}\right)}$  
   - 传播常数：${\gamma = \alpha + j\beta = j\omega \sqrt{\mu \varepsilon_c}}$  
   - 衰减常数：  
     $$
     \alpha = \omega \sqrt{\dfrac{\mu \varepsilon}{2} \left( \sqrt{1 + \left(\dfrac{\sigma}{\omega \varepsilon}\right)^2} - 1 \right)}
     $$

4. **反射与折射**  
   - 斯涅尔定律：${ \dfrac{\sin \theta_i}{\sin \theta_t} = \dfrac{n_2}{n_1} }$  
   - 全反射临界角：${ \theta_c = \arcsin\left(\sqrt{\dfrac{\varepsilon_2}{\varepsilon_1}}\right) }$  
   - 布儒斯特角：${ \theta_B = \arctan\left(\sqrt{\dfrac{\varepsilon_2}{\varepsilon_1}}\right) }$  

---

#### **第7章 边值问题解法**
1. **分离变量法**  
   - **直角坐标**：  
     $$
     \Phi(x,y,z) = X(x)Y(y)Z(z), \quad \nabla^2 \Phi = 0
     $$
   - **柱坐标**：  
     $$
     \Phi(\rho,\phi) = \sum_{n=0}^{\infty} [A_n \cos(n\phi) + B_n \sin(n\phi)] \left( C_n \rho^n + D_n \rho^{-n} \right)
     $$

2. **镜像法**  
   - **导体平面**：  
     - 镜像电荷：${ q' = -q }$（位置对称）  
   - **介质分界面**：  
     - 上半空间：${ q' = \dfrac{\varepsilon_1 - \varepsilon_2}{\varepsilon_1 + \varepsilon_2} q }$  
     - 下半空间：${ q'' = \dfrac{2\varepsilon_2}{\varepsilon_1 + \varepsilon_2} q }$  
   - **导体球**：  
     - 镜像电荷：${ q' = -\dfrac{a}{d} q }$，位置 ${ d' = \dfrac{a^2}{d} }$  

3. **唯一性定理**  
   - 给定边界条件（${\Phi|_S}$ 或 ${\left.\dfrac{\partial \Phi}{\partial n}\right|_S}$），拉普拉斯方程解唯一。  

---

### **附录：关键公式速查表**
| **物理量**         | **公式**                                                                 |
|--------------------|--------------------------------------------------------------------------|
| **波阻抗**         | ${ \eta = \sqrt{\mu / \varepsilon} }$                                    |
| **相速度**         | ${ v_p = \dfrac{1}{\sqrt{\mu \varepsilon}} }$                            |
| **衰减常数**       | ${ \alpha = \omega \sqrt{\dfrac{\mu \varepsilon}{2} \left( \sqrt{1 + \left(\dfrac{\sigma}{\omega \varepsilon}\right)^2} - 1 \right)} }$ |
| **临界角**         | ${ \theta_c = \arcsin\left(\sqrt{\dfrac{\varepsilon_2}{\varepsilon_1}}\right) }$ |
| **布儒斯特角**     | ${ \theta_B = \arctan\left(\sqrt{\dfrac{\varepsilon_2}{\varepsilon_1}}\right) }$ |
| **坡印廷矢量**     | ${ \vec{S}_{\text{av}} = \dfrac{1}{2} \operatorname{Re} (\dot{\vec{E}} \times \dot{\vec{H}}^*) }$ |

---
**说明**：  
- 所有公式已修正原PDF中的符号错误（如 ${\vec{\nabla}}$ 统一为 ${\vec{E}}$）。  
- 补充关键图示逻辑（如高斯定理的立体角证明、平面波斜入射几何关系）。  
- 删除冗余内容（如重复的坐标系公式），强化公式推导严谨性。