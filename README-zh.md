# units4TE
**热电领域中常见物理量的惯用单位总结**

> 选择语言：简体中文, [English](README.md)

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;在热电研究领域中，
有些物理量通常会使用一些非国际标准的惯用物理单位，
而且有的物理量可能存在多个惯用单位，比如对于导电性，
S/cm，10<sup>4</sup> S/m，μΩ·m 以及 mΩ·cm 等惯用单位都有被使用。
这对新手并不友好，尤其是在处理一些组合物理量时，
经常需要非常仔细的校对检查才能确保正确。
我们这里总结并约定了一些常见物理量的惯用单位，
给出常见组合参数的换算系数，既方便初学者能够快速熟悉这些惯用物理单位，
并且也倡导大家能够统一惯用单位以方便数据的直接对比和后处理程序的开发。
此外，还有一些物理量的惯用符号不但包含英文字符，
还包含一些希腊字符、拉丁字符以及上下标等扩展符号格式，
在一些文本编辑器中并不能够很好地被支持，
因此我们这里还约定了一套简单的纯英文字符来表示原先包含扩展字符的变量。
遵照这些约定，我们不但能够更加方便地设计程序处理接口，
还可以增强程序的可读性，从而提高程序开发者和使用者的工作效率。

- [Part I: 一些物理量的常用单位](#part-i-%E4%B8%80%E4%BA%9B%E7%89%A9%E7%90%86%E9%87%8F%E7%9A%84%E5%B8%B8%E7%94%A8%E5%8D%95%E4%BD%8D)
- [Part II: 一些常用的关系及其系数](#part-ii-%E4%B8%80%E4%BA%9B%E5%B8%B8%E7%94%A8%E7%9A%84%E5%85%B3%E7%B3%BB%E5%8F%8A%E5%85%B6%E7%B3%BB%E6%95%B0)
- [Part III: 单位换算关系](#part-iii-%E5%8D%95%E4%BD%8D%E6%8D%A2%E7%AE%97%E5%85%B3%E7%B3%BB)
- [Part IV: 数据模板](#part-iv-%E6%95%B0%E6%8D%AE%E6%A8%A1%E6%9D%BF)


### Part I: 一些物理量的常用单位

| 符号 | 扁平文本 | 单位 | 描述 |
| :----: | :-------: | ---- | ----------- |
| $T$ | T | K | 开氏绝对温度 |
| $\sigma$ | C | S·cm<sup>-1</sup> | 电导率 |
| $\rho$ | Rho | μΩ·m | 电阻率(= $1/\sigma$) |
| $S$ | S | μV·K<sup>-1</sup> | 塞贝克系数或者热电势 |
| $\kappa$ | K | W·m<sup>-1</sup>·K<sup>-1</sup> | 热导率 |
| $\theta$ or $R_{t}$ | Rth | m·K·W<sup>-1</sup> | 热阻率 (= $1/\kappa$ ) |
| $PF$ | PF | μW·cm<sup>-1</sup>·K<sup>-2</sup> | 功率因子 |
| $z$ | Z | K<sup>-1</sup> | 热电材料优值 |
| $ZT$ | ZT | 1 (dimensionless) | 无量纲热电优值 |
| $n$ | N | 10<sup>19</sup> cm<sup>-3</sup> | 载流子浓度 |
| $\mu$ | U | cm<sup>2</sup>·V<sup>-1</sup>·s<sup>-1</sup> | 载流子迁移率 |
| $m^{\ast}$ | meff | m<sub>e</sub> (=9.1093837015×10<sup>-31</sup> kg) | 载流子有效质量 |
| $L$ | LZ | 10<sup>-8</sup> V<sup>2</sup>·K<sup>-2</sup> (or 10<sup>-8</sup> W·Ω·K<sup>-2</sup>) | 洛伦兹常数 |
| $L$ | L | mm | 器件长度 |
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
| $v_{l}$ | vL | km·s<sup>-1</sup> | 纵向声速 |
| $v_{t}$ | vT | km·s<sup>-1</sup> | 横向声速 |
| $\tau$ | tau | ps (=10<sup>-12</sup> s) | 弛豫时间或粒子寿命 |
| $\nu$ or $f$ | freq | THz (=ps<sup>-1</sup>) | 圆频率 |
| $\omega$ | w | rad·ps<sup>-1</sup> (=THz) | 角频率(= $2\pi f$) |
| $T_{c}$ | Tc | K | 热端温度 |
| $T_{h}$ | Th | K | 冷端温度 |
| $\Delta T$ | DT | K | 温度差 (Th-Tc) |
| $s$ | CF | V<sup>-1</sup> | 相容性因子 |
| $(ZT)_{dev}$ | ZTdev | 1 (dimensionless) | 器件热电优值 |
| $(ZT)_{eng}$ | ZTeng | 1 (dimensionless) | 工程热电优值 |
| $(PF)_{eng}$ | PFeng | W·m<sup>-1</sup>·K<sup>-1</sup> | 工程功率因子 |
| $P_{d}$ | Pd | W·cm<sup>-2</sup> | 输出功率密度 |
| $\eta$ | Yita | % | 热电转化效率 |
| $Q_{hot}$ | Qhot |  W·cm<sup>-2</sup> | 热端热流密度 |
| $I$ | I | A | 工作电流 |
| $j$ | Jd | A·cm<sup>-2</sup> | 电流密度 |
| $R_{L}$ | RL | Ω | 负载电阻 |
| $V_{out}$ | Vout | mV | 输出电压 |
| $j_{sc}$ | Jsc | A·cm<sup>-2</sup> | 短路电流密度 |
| $V_{oc}$ | Voc | mV | 开路电压 |
| $R_{c}$ | Rc | μΩ·cm<sup>2</sup> (=10<sup>-10</sup> Ω·m<sup>2</sup>) | 接触电阻 |
| $\kappa_{c}$ | Kc | K·cm<sup>2</sup>·W<sup>-1</sup> | 接触热阻 |


### Part II: 一些常用的关系及其系数

- 电导率: `C = 1.6 N·U`
- 电阻率: `Rho = 1E4 /C`
- 功率因子: `PF = 1E-6 S^2·C = 1E-2 S^2/Rho`
- 无量纲热电优值: `ZT = 1E-10 (S^2·C)/K·T = 1E-4 PF/K·T`
- 相容性因子: `CF = 1E6 [sqrt(1+ZT)-1]/(S·T)`
- 开路电压: `Voc = 1E-3 S·DT`
- 短路电流密度: `Jsc = 1E-5 C·S·DT/L = 1E-1 S·DT/(Rho·L)`
- 热导率: `K = a·D·Cp` (换算系数恰好等于 1)
- 弹性常数: `Cii = D·vL^2` (换算系数恰好等于 1)
- 弛豫时间: `tau = 1/freq` (换算系数恰好等于 1)
- 玻尔兹曼常数 ( $k_{B}$ ): `8.6173E-5 eV/K`
- $k_{B}/e$ : `86.1733 μV/K`
- $k_{B}T$ @ 100 K: `8.6173 meV`
- $k_{B}T$ @ 300 K: `25.8520 meV`
- $k_{B}T$ 为 0.1 eV 时对应的温度: `1160.45 K`
- 金属的洛伦兹常数: `2.4430`


### Part III: 单位换算关系

- **Hartree 原子单位制**
    - 1 Bohr = 0.529 A
    - 1 Hartree = 27.211 eV = 2 Ry
- **压力**
    - 1 GPa = 10 kbar
    - 1 atm = 0.1013 MPa = 760 Torr(mmHg)
    - 1 Torr(mmHg) = 133.322 Pa
- **声子频率**
    - 1 THz = 4.136 meV = 33.356 cm<sup>−1</sup>
    - 1 meV = 0.242 THz = 8.066 cm<sup>−1</sup>
    - 1 cm<sup>−1</sup> = 0.030 THz = 0.124 meV
- **德拜温度和德拜频率**
    - 100 K ~ 2.08 THz
    - 1 THz ~ 47.99 K


### Part IV: 数据模板

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;这里展示了一个按列排放的数据模板（示例文件：
*[DataTemplate.txt](DataTemplate.txt)*
）。文件中每列数据对应一个物理量，具有相同的物理单位，而且每列的数据个数是一样的。
数据的分隔符可以是空格或者制表符，文件名以 .txt 为扩展名。
文件中以 "#" 号开头的行通常用来表示注解信息，比如日期，每列的变量名称、单位，
个人的备注信息等。这种格式的文件可以被绝大多数文本编辑器处理，而且可读性较好。

```
# Here are some comments. 
# Multiple lines of comments are allowed, but they must 
# all begin with the "#" character.
# Blank lines will be ignored (as shown below).

# property1   property2   property3   property4
300      0.0236       -51.33     9.3760e+01
323      0.0214       -40.33     9.9980e+01
373      0.0227       -8.53      9.6227e+01
423      0.0218        3.11      1.0170e+02
473      0.0228        18.29     9.7098e+01
523      0.0220        24.54     9.6694e+01
573      0.0217        54.92     1.0055e+02
623      0.0232        39.55     9.3134e+01
# Comments are also allowed to be inserted inside data blocks,
# as long as they start with a "#" sign as such.
673      0.0215        23.34     9.4004e+01
723      0.0235        0.13      8.3193e+01
773      0.0220       -16.76     9.7579e+01
823      0.0216       -48.61     9.9000e+01
873      0.0218       -93.34     1.0131e+02

# Here is a comment at the end of the file.
```

