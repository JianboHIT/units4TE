# units4TE
***Define a set of common units for thermoelectricity(TE)***

> Read this in other languages: [简体中文](README-zh.md), English

&nbsp;&nbsp;&nbsp;&nbsp;In thermoelectrics, some common units (non-SI units) 
are frequently used. For example, S/cm, 10<sup>4</sup> S/m, μΩ·m and mΩ·cm can all be used 
to characterize the electrical conductivity of a material and have been widely used. 
It is kind of unfriendly to beginners, especially when dealing with the combined physical properties, 
they have to spend a lot of time on careful proofreading. 
Here we define a set of common units and give the corresponding conversion factors 
for some typical combined physical properties. 
We expect this to be helpful to beginners, 
and highly recommend regarding them as the default physical units 
for the convenience of routine work and program interface design. 
In addition, we establish a set of plaintext symbols 
(excluding superscripts, subscripts and Latin characters) 
to indicate physical properties, which can be better supported by some text editors 
and enhances the readability of program scripts.

- [Part I: Common Units of Properties](#part-i-common-units-of-properties)
- [Part II: Useful Conversion Factors and Relationships](#part-ii-useful-conversion-factors-and-relationships)
- [Part III: Units Conversion](#part-iii-units-conversion)
- [Part IV: Data Template](#part-iv-data-template)


### Part I: Common Units of Properties

| Symbol | Plaintext | Unit | Description |
| :----: | :-------: | ---- | ----------- |
| $T$ | T | K | absolute temperature in Kelvin |
| $\sigma$ | C | S·cm<sup>-1</sup> | electrical conductivity |
| $S$ | S | μV·K<sup>-1</sup> | Seebeck coefficient or thermopower |
| $\kappa$ | K | W·m<sup>-1</sup>·K<sup>-1</sup> | thermal conductivity |
| $PF$ | PF | μW·cm<sup>-1</sup>·K<sup>-2</sup> | power factor |
| $z$ | Z | K<sup>-1</sup> | figure-of-merit of thermoelectric material |
| $ZT$ | ZT | 1 (dimensionless) | dimensionless figure-of-merit |
| $n$ | N | 10<sup>19</sup> cm<sup>-3</sup> | carrier concentration |
| $\mu$ | U | cm<sup>2</sup>·V<sup>-1</sup>·s<sup>-1</sup> | carrier mobility |
| $m^{*}$ | meff | m<sub>e</sub> (=9.1093837015×10<sup>-31</sup> kg) | carrier effective mass |
| $L$ | LZ | 10<sup>-8</sup> V<sup>2</sup>·K<sup>-2</sup> (or 10<sup>-8</sup> W·Ω·K<sup>-2</sup>) | Lorenz number |
| $L$ | L | mm | length of thermoelectric leg |
| $\rho$ | D | g·cm<sup>-3</sup> | density |
| $C_{p}$ | Cp | J·g<sup>-1</sup>·K<sup>-1</sup> | specific heat capacity at constant pressure |
| $C_{v}$ | Cv | J·g<sup>-1</sup>·K<sup>-1</sup> | specific heat capacity at constant volume |
| $a$ | a | mm<sup>2</sup>·s<sup>-1</sup> | thermal diffusivity |
| $a_{0}$ | a0 | Å (ångström, =10<sup>-10</sup> m) | lattice constant |
| $\Xi$ | Edef | eV | deformation potential constant |
| $C_{ii}$ | Cii | GPa (=10<sup>9</sup> Pa) | elastic constant |
| $\kappa_{e}$ | Ke | W·m<sup>-1</sup>·K<sup>-1</sup> | electronic thermal conductivity |
| $\kappa_{L}$ | KL | W·m<sup>-1</sup>·K<sup>-1</sup> | lattice thermal conductivity |
| $\kappa_{bip}$ | Kbip | W·m<sup>-1</sup>·K<sup>-1</sup> | bipolar thermal conductivity |
| $v$ | v | km·s<sup>-1</sup> | sound velocity |
| $v_{l}$ | vl | km·s<sup>-1</sup> | longitudinal sound velocity |
| $v_{t}$ | vt | km·s<sup>-1</sup> | transverse sound velocity |
| $\tau$ | tau | ps (=10<sup>-12</sup> s) | relaxation time or quantum lifetime |
| $\nu$ or $f$ | freq | THz (=ps<sup>-1</sup>) | ordinal frequency |
| $\omega$ | w | rad·ps<sup>-1</sup> (=THz) | angular frequency |
| $T_{c}$ | Tc | K | temperature at the cold side |
| $T_{h}$ | Th | K | temperature at the hot side |
| $s$ | CF | V<sup>-1</sup> | compatibility factor |
| $ZT_{device}$ | ZTdev | 1 (dimensionless) | device dimensionless figure-of-merit |
| $(ZT)_{eng}$ | ZTeng | 1 (dimensionless) | engineering dimensionless figure-of-merit |
| $(PF)_{eng}$ | PFeng | W·m<sup>-1</sup>·K<sup>-1</sup> | engineering power factor |
| $P_{d}$ | Pd | W·cm<sup>-2</sup> | output power density |
| $\eta$ | Yita | % | thermoelectric conversion efficiency |
| $Q_{hot}$ | Qhot |  W·cm<sup>-2</sup> | heat flux at the hot side |
| $I$ | I | A | load current |
| $j$ | Jd | A·cm<sup>-2</sup> | current density |
| $R_{L}$ | RL | Ω | load electric resistance |
| $V_{out}$ | Vout | mV | output voltage |
| $R_{c}$ | Rc | μΩ·cm<sup>2</sup> (=10<sup>-10</sup> Ω·m<sup>2</sup>) | electrical contact resistance |
| $\kappa_{c}$ | Kc | W·m<sup>-2</sup>·K<sup>-1</sup> | thermal contact conductance |


### Part II: Useful Conversion Factors and Relationships

- electrical conductivity: `C = 1.6 N·U`
- power factor: `PF = 1E-6 S^2·C`
- dimensionless figure-of-merit: `ZT = 1E-10 (S^2·C)/K·T = 1E-4 PF/K·T`
- thermal conductivity: `K = a·D·Cp` (factor is equal to 1)
- relaxation time: `tau = 1/freq` (factor is equal to 1)
- Boltzmann constant ( $k_{B}$ ): `8.6173E-5 eV/K`
- $k_{B}/e$ : `86.1733 μV/K`
- $k_{B}T$ at 100 K: `8.6173 meV`
- $k_{B}T$ at 300 K: `25.8520 meV`
- temperature where $k_{B}T$ is 0.1 eV: `1160.45 K`
- Lorenz number of metals: `2.4430`


### Part III: Units Conversion

- ***Hartree atomic units***
     - 1 Bohr = 0.529 A
     - 1 Hartree = 27.211 eV = 2 Ry
- ***pressure***
     - 1 GPa = 10 kbar
     - 1 atm = 0.1013 MPa = 760 Torr(mmHg)
     - 1 Torr(mmHg) = 133.322 Pa
- ***phonon frequencies***
     - 1 THz = 4.136 meV = 33.356 cm<sup>−1</sup>
     - 1 meV = 0.242 THz = 8.066 cm<sup>−1</sup>
     - 1 cm<sup>−1</sup> = 0.030 THz = 0.124 meV
- ***Debye temperature and Debye frequency***
     - 100 K ~ 2.08 THz
     - 1 THz ~ 47.99 K


### Part IV: Data Template

&nbsp;&nbsp;&nbsp;&nbsp;Here is a recommended template file to save 
column-indexed block-datas (see a example 
*[DataTemplate.txt](DataTemplate.txt)*
). Each column of data in the file corresponds to a property, 
they share the same unit, and the number of data samples in each column 
is the same. The file is delimited by spaces or tabs in the data block, 
and the filename has .txt as its extension. Lines starting with "#" in 
the file are usually interpreted as some comment information, such as date, 
author, variable name of each column, unit, personal comment information, etc. 
Data files in this format are highly readable and can be processed by most text editors.

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

