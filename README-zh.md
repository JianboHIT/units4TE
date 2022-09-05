# units4TE
约定一些热电领域中物理量的常用单位

- [Part I: Common Units of Properties](#part-i-common-units-of-properties)
- [Part II: Useful Conversion Factors and Relationships](#part-ii-useful-conversion-factors-and-relationships)
- [Part III: Units conversion](#part-iii-units-conversion)

### Part I: 一些物理量的常用单位

| 符号 | 扁平文本 | 单位 | 描述 |
| :----: | :-------: | ---- | ----------- |
| $T$ | T | K | 开氏绝对温度 |
| $\sigma$ | C | S·cm<sup>-1</sup> | 电导率 |
| $S$ | S | μV·K<sup>-1</sup> | 塞贝克系数或者热电势 |
| $\kappa$ | K | W·m<sup>-1</sup>·K<sup>-1</sup> | 热导率 |
| $PF$ | PF | μW·cm<sup>-1</sup>·K<sup>-2</sup> | 功率因子 |
| $z$ | Z | K<sup>-1</sup> | 热电材料优值 |
| $ZT$ | ZT | 1 (dimensionless) | 无量纲热电优值 |
| $n$ | N | 10<sup>19</sup> cm<sup>-3</sup> | 载流子浓度 |
| $\mu$ | U | cm<sup>2</sup>·V<sup>-1</sup>·s<sup>-1</sup> | 载流子迁移率 |
| $m^{*}$ | meff | m<sub>e</sub> (=9.1093837015×10<sup>-31</sup> kg) | 载流子有效质量 |
| $L$ | L | 10<sup>-8</sup> V<sup>2</sup>·K<sup>-2</sup> (or 10<sup>-8</sup> W·Ω·K<sup>-2</sup>) | 洛伦兹常数 |
| $\rho$ | D | g·cm<sup>-3</sup> | 密度 |
| $C_{p}$ | Cp | J·g<sup>-1</sup>·K<sup>-1</sup> | 定压比热 |
| $C_{v}$ | Cv | J·g<sup>-1</sup>·K<sup>-1</sup> | 定容比热 |
| $a$ | a | mm<sup>2</sup>·s<sup>-1</sup> | 热扩散系数 |
| $a_{0}$ | a0 | Å (ångström, =10<sup>-10</sup> m) | 晶格常数 |
| $\Xi$ | Edef | eV | 形变势 |
| $C_{ii}$ | Cii | GPa (=10<sup>9</sup> Pa) | 弹性常数 |
| $\kappa_{e}$ | Ke | W·m<sup>-1</sup>·K<sup>-1</sup> | 电子热导率 |
| $\kappa_{L}$ | KL | W·m<sup>-1</sup>·K<sup>-1</sup> | 晶格热导率 |
| $\kappa_{bip}$ | Kbip | W·m<sup>-1</sup>·K<sup>-1</sup> | 双极化热导率 |
| $v$ | v | km·s<sup>-1</sup> | 声速 |
| $v_{l}$ | vl | km·s<sup>-1</sup> | 纵向声速 |
| $v_{t}$ | vt | km·s<sup>-1</sup> | 横向声速 |
| $\tau$ | tau | ps (=10<sup>-12</sup> s) | 弛豫时间或粒子寿命 |
| $\nu$ or $f$ | freq | THz (=ps<sup>-1</sup>) | 圆频率 |
| $\omega$ | w | rad·ps<sup>-1</sup> (=THz) | 角频率 |
| $T_{c}$ | Tc | K | 热端温度 |
| $T_{h}$ | Th | K | 冷端温度 |
| $ZT_{eng}$ | ZTeng | 1 (dimensionless) | 工程热电优值 |
| $PF_{eng}$ | PFeng | μW·cm<sup>-1</sup>·K<sup>-2</sup> | 工程功率因子 |
| $P_{d}$ | Pd | W·cm<sup>-2</sup> | 输出功率密度 |
| $\eta$ | Yita | % | 热电转化效率 |
| $Q_{hot}$ | Qhot |  W·cm<sup>-2</sup> | 热端热流密度 |
| $I$ | I | A | 工作电流 |
| $j$ | Jd | A·cm<sup>-2</sup> | 电流密度 |
| $R_{L}$ | RL | Ω | 负载电阻 |
| $V_{out}$ | Vout | mV | 输出电压 |
| $R_{c}$ | Rc | μΩ·cm<sup>2</sup> (=10<sup>-10</sup> Ω·m<sup>2</sup>) | 接触电阻 |
| $\kappa_{c}$ | Kc | W·m<sup>-2</sup>·K<sup>-1</sup> | 接触热导 |

### Part II: 一些常用的关系及其系数
- 电导率: `C = 1.6 N·U`
- 功率因子: `PF = 1E-6 S^2·C`
- 无量纲热电优值: `ZT = 1E-10 (S^2·C)/K·T = 1E-4 PF/K·T`
- 热导率: `K = a·D·Cp` (换算系数恰好等于 1)
- 弛豫时间: `tau = 1/freq` (换算系数恰好等于 1)
- 玻尔兹曼常数 ( $k_{B}$ ): `8.6173E-5 eV/K`
- $k_{B}/e$ : `86.1733 μV/K`
- $k_{B}T$ @ 100 K: `8.6173 meV`
- $k_{B}T$ @ 300 K: `25.8520 meV`
- $k_{B}T$ 为 0.1 eV 时对应的温度: `1160.45 K`
- 金属的洛伦兹常数: `2.4430`

### Part III: 单位换算关系
- ***Hartree 原子单位制***
     - 1 Bohr = 0.529 A
     - 1 Hartree = 27.211 eV = 2 Ry
- ***压力***
     - 1 GPa = 10 kbar
     - 1 atm = 0.1013 MPa = 760 Torr(mmHg)
     - 1 Torr(mmHg) = 133.322 Pa
- ***声子频率***
     - 1 THz = 4.136 meV = 33.356 cm<sup>−1</sup>
     - 1 meV = 0.242 THz = 8.066 cm<sup>−1</sup>
     - 1 cm<sup>−1</sup> = 0.030 THz = 0.124 meV
- ***德拜温度和德拜频率***
     - 100 K ~ 2.08 THz
     - 1 THz ~ 47.99 K

