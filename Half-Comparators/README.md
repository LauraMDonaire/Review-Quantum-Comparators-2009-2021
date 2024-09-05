# Half - Comparators

## Overview

This section of the repository contains quantum half-comparators, which are particularly useful in quantum computing due to their ease of integration with algorithms such as Grover's algorithm.

## Circuits 

### Circuit 1: Thapliyal et al. (2010)
- **Authors**: H. Thapliyal, N. Ranganathan and R. Ferreira
- **Information**: Thapliyal et al. propose a **2-bit reversible comparator** and a **8-bit reversible comparator**.
  This first half-comparator is composed of two **R-Bcomp** units, one **CNOT** gate, and two **TR** gates. An **R-Bcomp** consists of two **TR** gates and one **CNOT** gate, and has a quantum cost of 31, a delay of 19△, a T-count of 14, a T-depth of 8, and two auxiliary inputs. Both circuits can be seen in **Figure 1**. 
<p align="center">
    <img src="https://github.com/LauraMDonaire/QuantumComparators/blob/main/Half-Comparators/Thapliyal%20et%20al.%202010/Thapliyals%20Quantum%20Half%20Comparator(n%3D2).png" alt="Thapliyal et al. proposed 2-bit reversible comparator" width="500"/>
</p>
<p align="center">
    <b>Figure 1: 2-bit Comparator proposed by Thapliyal et al. (2010)</b>
</p>
 
The second half-comparator proposed is composed of 7 **2-bit comparators** as nodes in a binary tree and a reversible output circuit (R-O/P Ckt). The output circuit is primarily used to generate the signal O2(x=y) from the outputs of x>y and x<y. To calculate the quantum cost of this comparator, the value of the 2-bit comparator is added to the value of the reversible output circuit, which is 9. This circuit can be seen in **Figure 2**. 

<p align="center">
    <img src="https://github.com/LauraMDonaire/QuantumComparators/blob/main/Half-Comparators/Thapliyal%20et%20al.%202010/Thapliyals%20Quantum%20Half%20Comparator(n%3D8).png" alt="Thapliyal et al. proposed 8-bit reversible comparator" width="500"/>
</p>
<p align="center">
    <b>Figure 2: 8-bit Comparator proposed by Thapliyal et al. (2010)</b>
</p>

The metrics of this circuits can be seen in **Table 1**. 

- **IBM Quantum Platform**: [View Circuit (n=2) on IBM Quantum Platform](https://quantum-computing.ibm.com/...)

### Circuit 2: Xia et al. (2018)
- **Authors**: H. Xia, H.-S. Li, and H. Zhang
- **Information**: The 6-bit comparator proposed by Xia et al. in 2018 is shown in Figure 3. This comparator is composed of 48 CNOT gates and 24 Toffoli gates, all of which have negated controls. With negated controls (which is equivalent to two Pauli-X gates), the quantum cost of each gate is 7, and the delay increases to 7∆.

<p align="center">
    <img src="https://github.com/LauraMDonaire/QuantumComparators/blob/main/Half-Comparators/Xia%20et%20al.%202018/Xias%20Quantum%20Half%20Comparator(n%3D6).png" alt="Xia et al. proposed 6-bit comparator" width="500"/>
</p>
<p align="center">
    <b>Figure 3: 6-bit Comparator proposed by Xia et al. (2018)</b>
</p>
  
The metrics of this circuit can be seen in **Table 1**. 
- **IBM Quantum Platform**: [View Circuit on IBM Quantum Platform](https://quantum-computing.ibm.com/...)

### Circuit 3: Xia et al. (2019)
- **Authors**: H. Xia, H.-S. Li, H. Zhang, Y. Liang, and J. Xin
- **Information**: The first half-comparator proposed by Xia et al. (2019) is the 1-bit comparator (see **Figure 4**). This comparator consists of a single **Toffoli** gate with a negated control. In this half-comparator, the relationship between `a0`, `b0`, and `c0` is given by |c0⟩ = |0⟩ |A¯0b0⟩.
<p align="center">
    <img src="https://github.com/LauraMDonaire/QuantumComparators/blob/main/Half-Comparators/Xia%20et%20al.%202019/Xias%20Quantum%20Half%20Comparator(n%3D1)%202019.png" alt="Xia et al. (2919) proposed 1-bit comparator" width="500"/>
</p>
<p align="center">
    <b>Figure 4: 1-bit Comparator proposed by Xia et al. (2019)</b>
</p>
  

Additionally, they propose a 2-bit half-comparator. This comparator includes 7 **CNOT** gates and three **Toffoli** gates, one of which has a negated control. This comparator can be seen in **Figure 5**.
<p align="center">
    <img src="https://github.com/LauraMDonaire/QuantumComparators/blob/main/Half-Comparators/Xia%20et%20al.%202019/Xias%20Quantum%20Half%20Comparator(n%3D2)%202019.png" alt="Xia et al. proposed 2-bit comparator" width="500"/>
</p>
<p align="center">
    <b>Figure 5: 2-bit Comparator proposed by Xia et al. (2010)</b>
</p>
  
Similar to the 2-bit half-comparator, they also propose a 3-bit half-comparator. This comparator adds two **Toffoli** gates with negated controls and four **CNOT** gates. This comparator can be observed in **Figure 6**.
<p align="center">
    <img src="https://github.com/LauraMDonaire/QuantumComparators/blob/main/Half-Comparators/Xia%20et%20al.%202019/Xias%20Quantum%20Half%20Comparator(n%3D3)%202019.png" alt="Xia et al. proposed 3-bit comparator" width="500"/>
</p>
<p align="center">
    <b>Figure 6: 3-bit Comparator proposed by Xia et al. (2019)</b>
</p>
  
To create the 4-bit half-comparator (see Figure 7), 15 **CNOT** gates and 7 **Toffoli** gates are used, with 5 of the **Toffoli** gates having a negated control.
<p align="center">
    <img src="https://github.com/LauraMDonaire/QuantumComparators/blob/main/Half-Comparators/Xia%20et%20al.%202019/Xias%20Quantum%20Half%20Comparator(n%3D4)%202019.png" alt="Xia et al. proposed 4-bit comparator" width="500"/>
</p>
<p align="center">
    <b>Figure 7: 4-bit Comparator proposed by Xia et al. (2019)</b>
</p>
  
The 8-bit half-comparator (see Figure 8) consists of 23 **CNOT** gates and 15 **Toffoli** gates, with 13 of the **Toffoli** gates having a negated control.
<p align="center">
    <img src="https://github.com/LauraMDonaire/QuantumComparators/blob/main/Half-Comparators/Xia%20et%20al.%202019/Xias%20Quantum%20Half%20Comparator(n%3D8)%202019.png" alt="Xia et al. proposed 8-bit comparator" width="500"/>
</p>
<p align="center">
    <b>Figure 8: 8-bit Comparator proposed by Xia et al. (2019)</b>
</p>
  
The metrics of this circuits can be seen in **Table 1**. 
- **IBM Quantum Platform**: [View Circuit on IBM Quantum Platform](https://quantum-computing.ibm.com/...)

### Circuit 4: Li et al. (2020) 
- **Authors**: H.-S. Li, P. Fan, H. Xia, H. Peng, and G. Long
- **Information**: The recreated half-comparator proposed by Li et al. for n=3 is composed of 8 **CNOT** gates and 5 **TR** gates (see **Figure 9**).
  <p align="center">
    <img src="https://github.com/LauraMDonaire/QuantumComparators/blob/main/Half-Comparators/Li%20et%20al.%202020/Lis%20Quantum%20Half%20Comparator(n%3D3).png" alt="Li et al. proposed a 3-bit comparator" width="500"/>
</p>
<p align="center">
    <b>Figure 9: 3-bit Comparator proposed by Li et al.</b>
</p>

The metrics of this circuit can be seen in **Table 1**. 

- **IBM Quantum Platform**: [View Circuit on IBM Quantum Platform](https://quantum.ibm.com/composer/files/new?initial=N4IgdghgtgpiBcIAyBLABDALmiAbAdGgBRgC8AzAJRoC0AygBICCASgKIAiIANCAI4QAzlAQgA8gAU2AOQCKTOgFk0AJnwAGANwAdMCjABjXAFcAJjDTb%2BMXCgBGARnz6DVnWADmETBYMA1HG40OzRgXTQ0bAh3CIALYJi0AwAPYKDo8MjTDxxE7DtElLTczPiC3QBfXS8fJL8JQODQ0oTMort0vJKwCMxs1p6k1I7u3v6MwbL3Ks9vC0wWB0aRg2bB-waVxIBhAA1lwoCIIIND4tPK6rnIlhVlk7WI-0aLwb3iiaf687PjpOmrrUAE4AIQMAHsoAAHe5JIKmR43JZ-EamQqpFF5W6w14zGrzFjkHGIjYHNqpAydNpHILldYBSkDPHXBYAFmJYXpmypb32jLpXw%2BZ0ZE2ZtShMCBMEEyNpD05gpFZxGnzQ735hwamMus3FkulHOpWpOypN5LJ9J%2BOr4UpyfAA2gB2AC67gMtqSTtdul0UsEWDQDvU3rA8QdDhDYftKkjgft5FjDtZiftAFYUwA2EN2CBAoEoSVx4NBcPOkvRstxhPl5Pl9PlrPud4OmPliNN-ZJysOhMduOtosh5v22v97O5-OFoPd%2B0R8sDnsz0cO%2Btxxu6UkrpdDzv2rN1kPPLc1w8BB37uPJ9w5vMFoGDtszhfx7cHhunhqL%2Bc7y8z3sbs8X2-N1AOXCtrwnO8HzjOcx3LatfzfNcPxgmdgz7FsZ3bADUPLdCcMwvDx1vKd7WLXC4KrV841Xc8f0I1CIJI%2B9p0fb94Oo49kJAxCxx4r8%2BN0YcwP-QxvgEzCmMnFiyKwp8-04tMZ3XMTkJPfilPUoTdwvLcQM-TTfykqDWIohiJJHGdaL3Q9Ui7YDtMo0sMMsjjjNI8jS3YqiTyQuj3FgIRjClQdaAAPk9fCwECwRgosUtws9bDopgIKQswxKDHA3QYriqjMpfALUti9LLIKq8cuKvKtwK9MirS%2BKbIKlTdAAelatAAAEIRMKAwEENAyO4dRhtGkbxu4BxuBUabuHIbhWW4VNuAzbhHW4AAObgAE5JpGhwpocGaHHmhxFocZaHFWhx1ocLaHF2lQRpUKaVBmlR5pURaVGWlRVpUdaVC2lRdvIEbyCm8gZvIebyEWuG5uW8hVvIdbyC28hdtZEbWSm1kY10HgQHMQR3RQKFMBQcEwFEEAKiAA)

### Circuit 4: Orts et al. (2021) 
- **Authors**: F. Orts, G. Ortega, A.C. Cucura, E. Filatovas and E.M. Garzón
- **Information**: The first half-comparator (see **Figure 10**) proposed by Orts et al. is based on the methodology of the adder devolep in [1], which is the best adder available in terms of T-count. The comparison between the two bit strings `a` and `b` is performed using the operation `a - b`. This operation can be executed using an adder by computing `a + ¯b`. Currently, only the sign of the operation is of interest. It can be determined that `a` is less than `b` if the sign of `a - b` is negative, or that `a` is greater than (or equal to) `b` if the result is positive. In the comparison, this half-comparator will be referred to as the Orts et al. comparator (a). This comparator has 4 **Temporary-logical AND** gates, 17 **CNOT** gates, 8 **Pauli-X** gates, and 3 **Temporary-logical AND** gate decomputation gates. 
  <p align="center">
    <img src="https://github.com/LauraMDonaire/QuantumComparators/blob/main/Half-Comparators/Orts%20et%20al.%202021/Ortss%20Quantum%20Half%20Comparator(n%3D4).png" alt="Orts et al. proposed a 4-bit comparator" width="500"/>
</p>
<p align="center">
    <b>Figure 10: 4-bit Comparator proposed by Orts et al.</b>
</p>

The second comparator proposed by Orts et al. (see **Figure 11**) is based on the adder developed in [2], which is currently the best adder available in terms of T-depth [3]. Again, the comparison of this circuit is performed using the function `a + ¯b`. This circuit implements the use of a large number of auxiliary qubits to achieve logarithmic T-depth, as each operation is performed using **Temporary-logical AND** gates. These gates could be fully or partially replaced to reduce the number of auxiliary inputs. However, this would increase the T-depth and T-count of the circuit. This half-comparator will be referred to as the Orts et al. comparator (b) in the comparison. This comparator is composed of 19 **Temporary-logical AND** gates, 16 **Pauli-X** gates, 21 **CNOT** gates, and 18 **Temporary-logical AND** gate decomputation gates.

  <p align="center">
    <img src="https://github.com/LauraMDonaire/QuantumComparators/blob/main/Half-Comparators/Orts%20et%20al.%202021/Ortss%20Quantum%20Half%20Comparator(n%3D8).png" alt="Orts et al. proposed a 8-bit comparator" width="500"/>
</p>
<p align="center">
    <b>Figure 11: 8-bit Comparator proposed by Orts et al.</b>
</p>

The metrics of this circuits can be seen in **Table 1**. 
- **IBM Quantum Platform**: [View Circuit (n=4) on IBM Quantum Platform](https://quantum.ibm.com/composer/files/new?initial=N4IgdghgtgpiBcIDyAnALgZwAQzViANgHRYAUYAvACwCUWAtFgMoASAggEoCiAIiADQgAjhAxQEyAApcAcgEU2TALJYATEQAMAbgA6YAJZgAxgQCuAExhYdwmAX0AjAIxFDRm7rABzCGit%2BoAAcAexQIFABPNjBzfH4sB3ijLGA9LCwjAA84jM90rISkvIzso3iHYoKy-GK0cy8atKw6hoqmvCNigGEADQz4iErS8uKAC1ym7E69AF89IRQYBqEAbSdVAF1PI0WGozWNLb09cdXDz1O1o7BLzYusVYBma8uqF4eVgFZ31YA2H5WAHYAQAOAEATgBTnOJw%2BTic1zwqzueiRX0RHzBnjR8OuDnCKH0MBQH0O8VWCPJK02VOeVLeVO%2BVP%2BVOBVLBVMhVOhG25CM82TO10FK2eAo%2B-3Fq0hnnxKEJxNJvLhyuRqtF6oZHyZEvVbMx6q5cLJcP5egKQqpKOMIspH2tFup6rNNvt6phYBaSux9RV2Ldnl6bqpHsdNL9sLVnmwUb0coVJMtKqt6rpHy1qx1fz16o5HyNFJNFJdYdT11L9LxBKJiZWRauKdpmvVWZWLI%2B%2BtWeelzvruO2IrTmfLIoz6IH2ubE%2BHTZ9yw1c-TGOHgb6M4%2BYvNItbb3uK70MfHceriqTFPV4aezcZ6vbq07K27KwLB2dJZFl6PrvX2en6NZVbyjWSrcheZaVjezI5uyhq9m%2BI66jBf4PliW4GgBf5PpKqK%2Br%2BOHzsC-pdtcQbEVBmE5nuj7XIeqFgPGwFng2wYbtek5QQBMGcnBfIIT%2B1EUdxgnGoBCYgcmLFXhB7GIR2uawdyfbvvm8F-jyvFqXahZ8WsWnPoiuH6Yu2lEbpJFrmZQlocWcFUf2B6mqJjF1s6YFNtJ-F3kC8ncYpqnWdRGkBU%2BPLCT2f6tnRDGni5oGNqxHn-rJ94%2BSpflBd%2Bbbych2XBZReXkfhurGd5pl0aRgXFQVclUXRtFOTFfZuQlS6Qcl3lcWlIkZY6raEQFrbYZln7fLKJ61k18VSa1MnZpx6FddpPWDi2OljqNA1Tpts5FVeJW7qik6rrNC7bUuVEbWAh6XdFE2uVNGqJYN0ELT26WOWpW3DWWY1AY192SY9M2eS9ZGLa%2By3ibGmV6Q6H6uX%2Bn4el6QolS6aLWhVSM6Z%2BLq3DRAbHn9d1xYDQ4rOtt6g5Vb3dR9egih6K1SllLMykTYlMbD4HA0lc1yZ1tNLfTYCwKIpiLEqDAAHwZC5nhixgEtWOeMtyy6ivK26av7NamuS1eOunaLMDiwbFMbEbB0m2bKvokbl363b-xG0NTtyUb-U20r5tgkbdHuz2Rvs97WvacH1yB2ZEeeHoAD0cdYAAAkYwRmFAV1YHW-AaDnee5wX%2BdF7nTj8KX5f8Ko-CPNXtc11Q-CfPwvz8IC-Agvw4Kd930Jl%2BXVdODXTgN04TdOC3Tht04HdOF3qi56opeqFXy%2BVyvNeqA3qhN6oLeqG3qgd6oXePLnjyl48VePDXjwN48TePC3j-V0-bePB3jxd1QudUKXVBV1QeuDcqBNyoC3KgbcqAdyoF3T4uc4GN3gaXT4VdPg10%2BA3T4TdPgt0%2BG3T4HdPhd1%2BLnX4pdfhV1%2BDXX4DdfhNzoc3ehLdfht1%2BB3X4XdAS50BKXQEVdAQ10BA3QETdAQt0BG3QEHdAScNke3XOIJS4giriCGuIIG4gibiCFuII24gg7iCLu4Jc7glLuCKu5jO4WJruCBu4Im7ghbuCNu4IO6uM7m4txXdoQlw0OXDQA8NBDw0CPDQY8NATw0FPDQM8NDeN7vCBEegBAgEsBgHY%2BhAhoH0MEMAEgQAzCAA)

- [1] C. Gidney, “Halving the cost of quantum addition,” Quantum, vol. 2, p. 74, 2018.
- [2] H. Thapliyal, E. Muñoz-Coreas, and V. Khalus, “T-count and qubit optimized quantum circuit designs of carry lookahead adder,” 2020.
- [3] F. Orts, G. Ortega, E. Fernández-Combarro and E.M. Garzón, “A review on reversible quantum adders,” Journal of Network and Computer Applications, 2020.
## Metrics

The following table summarizes the quantum cost metrics for the half-comparator circuits, evaluated for various values of $n$. Please note that these metrics are based on general implementations of the quantum gates used in each circuit. For accurate reproduction of these results, understanding the specific context and details of the gate implementations is essential. Feel free to reach out to me for any questions or further clarification regarding these implementations.

| Circuit                | Size of n        | Quantum Cost | Delay | T-count | T-depth | Ancillary Inputs |
|------------------------|------------------|--------------|-------|---------|---------|------------------|
| Thapliyal et al. (2010)| 2                | 27           | 18    | 54      | 36      | 4                |
| Thapliyal et al. (2010)| 8                | 198          | 61    | 378     | 108     | 15               |
| Xia et al. (2018)      | 6                | 216          | 174   | 168     | 72      | 3                |
| Xia et al. (2019)      | 1                | 7            | 7     | 7       | 3       | 1                |
| Xia et al. (2019)      | 2                | 24           | 21    | 21      | 9       | 2                |
| Xia et al. (2019)      | 3                | 40           | 35    | 35      | 15      | 2                |
| Xia et al. (2019)      | 4                | 60           | 49    | 49      | 21      | 2                |
| Xia et al. (2019)      | 8                | 124          | 105   | 105     | 45      | 2                |
| Li et al. (2020)       | 3                | 83           | 51    | 35      | 20      | 1                |
| Orts et al. (2021) (a) | 4                | 78           | 64    | 16      | 8       | 4                |
| Orts et al. (2021) (b) | 8                | 289          | 66    | 76      | 38      | 19               |

**Table 1: Metrics for Half-Comparators studied for specific values of n.**




## How to Use

Each circuit in this directory includes an analysis of the gates used, a visual diagram, and a link to its implementation on the IBM Quantum Platform. You can explore each circuit individually by following the links provided.
