### 电磁场与电磁波期末模拟试题

#### 一、选择题（每题3分，共15分）
1. 关于导体静电平衡，**错误**的说法是：  
   A. 导体内部电场为零  
   B. 导体表面是等势面  
   C. 电荷仅分布在导体表面  
   D. 导体表面电场方向与表面成45°角  

2. 恒定磁场中，矢量磁位${\vec{A}}$满足的方程是：  
   A. ${\nabla \times \vec{A} = \vec{B}}$  
   B. ${\nabla^2 \vec{A} = -\mu \vec{J}}$  
   C. ${\nabla \cdot \vec{A} = \rho}$  
   D. ${\vec{A} = \frac{\mu_0 I}{4\pi r}}$  

3. 平面波从空气（${\eta_1 = 377 \Omega}$)垂直入射到玻璃（${\eta_2 = 188.5 \Omega}$)，反射系数为：  
   A. 0.33  
   B. -0.33  
   C. 0.67  
   D. -0.67  

4. 麦克斯韦方程组中，位移电流的贡献体现在：  
   A. ${\nabla \times \vec{E} = -\frac{\partial \vec{B}}{\partial t}}$  
   B. ${\nabla \times \vec{H} = \vec{J} + \frac{\partial \vec{D}}{\partial t}}$  
   C. ${\nabla \cdot \vec{D} = \rho}$  
   D. ${\nabla \cdot \vec{B} = 0}$  

5. 全反射临界角${\theta_c}$的计算公式是：  
   A. ${\theta_c = \arcsin(\sqrt{\epsilon_2/\epsilon_1})}$  
   B. ${\theta_c = \arctan(\sqrt{\mu_2/\mu_1})}$  
   C. ${\theta_c = \arccos(\epsilon_2/\epsilon_1)}$  
   D. ${\theta_c = \arcsin(\mu_1/\mu_2)}$  

---

#### 二、填空题（每空2分，共20分）
1. 真空中点电荷${q}$产生的电位${\Phi = }$ ______，电场强度${\vec{E} = }$ ______。  
2. 线性介质中极化强度${\vec{P}}$与电场的关系是______。  
3. 安培环路定律的微分形式：______。  
4. 自由空间平面波的波阻抗${\eta = }$ ______Ω，相速度${v_p = }$ ______m/s。  
5. 坡印廷矢量的瞬时表达式是______，平均功率密度是______。  
6. 导体球镜像法中，镜像电荷量${q' = }$ ______，位置${d' = }$ ______。  

---

#### 三、计算题（共45分）
1. **(10分)** 同心球电容器内半径${R_1=2\text{cm}}$，外半径${R_2=5\text{cm}}$，介质${\epsilon_r=3}$，带电量${Q=1\mu\text{C}}$。  
   (1) 求电场分布${E(r)}$  
   (2) 计算电容值  
   (3) 求储能${W_e}$

2. **(10分)** 无限长直导线电流${I=10\text{A}}$，距导线${d=0.5\text{m}}$处：  
   (1) 求磁感应强度${\vec{B}}$  
   (2) 计算矢量磁位${\vec{A}}$  
   (3) 若平行放置另一相同导线（同向电流），求单位长度受力

3. **(10分)** 空气中均匀平面波：${\vec{E} = 100\cos(10^8 t - \beta z) \vec{e_x} \text{V/m}}$  
   (1) 求${\beta}$和波长${\lambda}$  
   (2) 写出磁场${\vec{H}}$表达式  
   (3) 计算平均坡印廷矢量${\vec{S}_{av}}$

4. **(15分)** 平面波从空气（区域1）斜入射到理想导体（区域2），${\theta_i=30^\circ}$，${E_0=100\text{V/m}}$（垂直极化）：  
   (1) 求反射系数${\Gamma}$  
   (2) 写出空气中合成波${\vec{E}}$的表达式  
   (3) 求导体表面感应电流密度${\vec{J}_s}$

---

#### 四、证明题（每题10分，共20分）
1. 由麦克斯韦方程组推导无源区波动方程：${\nabla^2 \vec{E} - \mu\epsilon \frac{\partial^2 \vec{E}}{\partial t^2} = 0}$

2. 证明两种介质分界面上：${E_{1t} = E_{2t}}$（电场切向分量连续）

---

### 答案及解析

#### 一、选择题
1. **D**（导体表面电场垂直于表面）  
2. **B**（矢量磁位泊松方程）  
3. **B**（${\Gamma = \frac{\eta_2-\eta_1}{\eta_2+\eta_1} = \frac{188.5-377}{188.5+377} \approx -0.33}$)  
4. **B**（位移电流在安培定律修正项中）  
5. **A**（临界角定义公式）  

#### 二、填空题
1. ${\frac{q}{4\pi\epsilon_0 r}}$；${\frac{q}{4\pi\epsilon_0 r^2}\hat{e_r}}$  
2. ${\vec{P} = \epsilon_0 \chi_e \vec{E}}$  
3. ${\nabla \times \vec{H} = \vec{J}}$  
4. ${377}$；${3 \times 10^8}$  
5. ${\vec{S} = \vec{E} \times \vec{H}}$；${\vec{S}_{av} = \frac{1}{2} \text{Re}(\vec{E} \times \vec{H}^*)}$  
6. ${-\frac{a}{d}q}$；${\frac{a^2}{d}}$  

#### 三、计算题
1. **(1)** ${E(r) = \frac{Q}{4\pi\epsilon r^2} = \frac{10^{-6}}{4\pi \times 3\epsilon_0 r^2}}$  
   **(2)** ${C = 4\pi\epsilon \frac{R_1 R_2}{R_2-R_1} = 4\pi \times 3\epsilon_0 \frac{0.02 \times 0.05}{0.03} \approx 1.11 \times 10^{-10}\text{F}}$  
   **(3)** ${W_e = \frac{Q^2}{2C} = \frac{(10^{-6})^2}{2 \times 1.11 \times 10^{-10}} \approx 4.5 \times 10^{-3}\text{J}}$  

2. **(1)** ${B = \frac{\mu_0 I}{2\pi d} = \frac{4\pi \times 10^{-7} \times 10}{2\pi \times 0.5} = 4 \times 10^{-6}\text{T}}$  
   **(2)** ${\vec{A} = \frac{\mu_0 I}{4\pi} \ln \frac{\rho_0}{\rho} \hat{e_z}}$（需选参考点）  
   **(3)** ${F = \frac{\mu_0 I^2}{2\pi d} = \frac{4\pi \times 10^{-7} \times 100}{2\pi \times 0.5} = 4 \times 10^{-5}\text{N/m}}$  

3. **(1)** ${\beta = \omega \sqrt{\mu_0\epsilon_0} = \frac{10^8}{3 \times 10^8} = \frac{1}{3} \text{rad/m}}$，${\lambda = \frac{2\pi}{\beta} = 6\pi \text{m}}$  
   **(2)** ${H_y = \frac{E_x}{\eta_0} = \frac{100}{377} \cos(10^8 t - \beta z)}$  
   **(3)** ${\vec{S}_{av} = \frac{1}{2} \frac{E_0^2}{\eta_0} \hat{e_z} = \frac{1}{2} \frac{10000}{377} \hat{e_z} \approx 13.26 \hat{e_z} \text{W/m}^2}$  

4. **(1)** ${\Gamma = -1}$（理想导体）  
   **(2)** 合成波：  
   $$
   \vec{E} = -2j E_0 \sin(k z \cos\theta_i) e^{-j k x \sin\theta_i} \hat{e_y}
   $$  
   **(3)** ${\vec{J}_s = \hat{n} \times \vec{H}|_{z=0} = \frac{2E_0}{\eta_0} \cos\theta_i \hat{e_x}}$  

#### 四、证明题
1. **证明**：  
   ${\nabla \times (\nabla \times \vec{E}) = \nabla \times (-\frac{\partial \vec{B}}{\partial t}) = -\mu \frac{\partial}{\partial t} (\nabla \times \vec{H})}$  
   代入${\nabla \times \vec{H} = \frac{\partial \vec{D}}{\partial t}}$得：  
   ${\nabla (\nabla \cdot \vec{E}) - \nabla^2 \vec{E} = -\mu \epsilon \frac{\partial^2 \vec{E}}{\partial t^2}}$  
   无源区${\nabla \cdot \vec{E} = 0}$，故${\nabla^2 \vec{E} - \mu\epsilon \frac{\partial^2 \vec{E}}{\partial t^2} = 0}$  

2. **证明**：  
   在分界面取矩形回路（高${\Delta h \to 0}$），由：  
   ${\oint \vec{E} \cdot d\vec{l} = E_{1t} \Delta l - E_{2t} \Delta l = 0}$  
   得${E_{1t} = E_{2t}}$  

---

> **刷题建议**：  
> 1. 静电场重点练高斯定理应用（球/柱对称场）  
> 2. 磁场掌握安培定律和矢量磁位计算  
> 3. 平面波必考反射系数和极化计算  
> 4. 证明题理解麦克斯韦方程物理意义  
> 做完后对照答案订正，薄弱环节重点突破！