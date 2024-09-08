# Full Comparators

## Overview

This section of the repository contains the study of some quantum full comparators. Although the primary focus of this work is on semi-comparators, for the sake of clarity, the full comparators mentioned in the articles by Xia et al. (2019) and Al-Rabadi (2009) have also been analyzed. This is because these works do not clearly distinguish between the types of comparators, which has led me to examine all the circuits included. However, only the semi-comparators will be considered in the final analysis.

## Circuits 

### Circuit 1: Al-Rabadi (2009)
- **Authors**: A. Al-Rabadi
- **Information**: Al-Rabadi propose a **full comparator** composed by nine **Pauli-X** gates, and six **Toffoli** gates. 
<p align="center">
    <img src="https://github.com/LauraMDonaire/Review-Quantum-Comparators-2009-2021/blob/main/Full%20Comparators/Al-Rabadi%20(2009)/Al-Rabadi's%20Comparator.png" alt="Al-Rabadi proposed comparator" width="500"/>
</p>
<p align="center">
    <b>Figure 1: On the left, the full comparator proposed by Al-Rabadi and its output on the right side.</b>
</p>

The metrics of this circuit can be seen in **Table 1**. 

- **IBM Quantum Platform**: [View Circuit on IBM Quantum Platform](https://quantum.ibm.com/composer/files/new?initial=N4IgdghgtgpiBcICCAbAtAJQgIwgEwEsQAaEARwgGcoEQB5ABQFEA5ARSQGUBZAAgCYAdAAYA3AB0wBMAGMUAVzwxe48jBQFsARkHSZqiWElkATjADmvMgG0tWgLqGZZyzNsPDkgBZXrwx96%2BHpJmlDAALr78AWA%2BNgDMMXHWACwxoRG%2BAKzpMGGRNgBsufm%2BAOwlmTYAHJUF1gCcdUH%2BhrgmJgQwJr7%2BxEH2-TbRQ9aJo2mjOaPFoxWjtaNNhgAevTFrCTEyMpt%2BgwOj0W0QHV09Nn2HUQdbE7fW076z5Q%2BLvsuSe61fA6u%2BaScuxu9ymG2yMXanW661GDiOD3GAIeTyKD3mvneNk%2BsmBlwe8Oe2zxYweLxsFSBeyRNlR1lq-wpxL2k1eS0hp2hF32cIeI18NNSKLJ6LeDxxewZv2xHLOMPxvIRo0FrNpIrmYvZjPp4JlVMx4oJPzAkt1jRisCo8jMLXsvDQAD5eG4tMaoedYddhoiHqrHuq2QatZJLZRrcp8fanW5jaHwwMo87bBaYFabd7E25jiHU2H06TM6TDHH82lC4Cc2mI-7Czli7n42jC8V61XXoXKZW89XaoWpWAS9WmoWcZIAPRj3gAARkAHsFFAwJReH5iMI1xv11vNzutMR%2BPviPFiCliFkzxfCsQysRqsQGsRXY%2B91oD1pj1pT1pz9-H1etDeAGPneWgPqBj4Pvw678Hu-AHvwx78Ke-DnvwV78De-B3vwD7xP4kgkCASiUM4BAAA7hAQs5gLQIAAL5AA)

- **Reference**: A. Al-Rabadi, “Closed-system quantum logic network implementation of the Viterbi algorithm,” *Facta Universitatis. Series Electronics and Energetics*, vol. 22 (1), pp. 1–33, 2009. [DOI:10.2298/FUEE0901001A](https://doi.org/10.2298/FUEE0901001A)


### Circuit 3: Xia et al. (2019)
- **Authors**: H. Xia, H.-S. Li, H. Zhang, Y. Liang, and J. Xin
- **Information**: The first full comparator found is a 1-bit full comparator (it can be seen in **Figure 2**). This comparator consists of 2 **CNOT** gates and 2 **Toffoli** gates, one of which has a negated control.

<p align="center">
    <img src="https://github.com/LauraMDonaire/Review-Quantum-Comparators-2009-2021/blob/main/Full%20Comparators/Xia%20et%20al.%202019/Xias%20Quantum%20Full%20Comparator%20(n%3D1).png" alt="Xia et al. (2019) proposed 1-bit comparator" width="500"/>
</p>
<p align="center">
    <b>Figure 2: 1-bit Full Comparator proposed by Xia et al. (2019)</b>
</p>

Xia et al. also propose a 2-bit full comparator. This comparator has 7 **CNOT** gates and 5 **Toffoli** gates, 2 of which have a negated control. This 2-bit full comparator can be seen in **Figure 3**.
<p align="center">
    <img src="https://github.com/LauraMDonaire/Review-Quantum-Comparators-2009-2021/blob/main/Full%20Comparators/Xia%20et%20al.%202019/Xias%20Quantum%20Full%20Comparator%20(n%3D2).png" alt="Xia et al. proposed 2-bit comparator" width="500"/>
</p>
<p align="center">
    <b>Figure 2: 2-bit Full Comparator proposed by Xia et al. (2019)</b>
</p>
  
The next full comparator is a 3-bit one (see **Figure 4**). It has 12 **CNOT** gates and 7 **Toffoli** gates, 5 of which have a negated control.

<p align="center">
    <img src="https://github.com/LauraMDonaire/Review-Quantum-Comparators-2009-2021/blob/main/Full%20Comparators/Xia%20et%20al.%202019/Xias%20Quantum%20Full%20Comparator%20(n%3D3).png" alt="Xia et al. proposed 3-bit comparator" width="500"/>
</p>
<p align="center">
    <b>Figure 4: 3-bit Full Comparator proposed by Xia et al. (2019)</b>
</p>

Another proposed full comparator is the 4-bit one (see **Figure 5**). This comparator has 15 **CNOT** gates and 9 **Toffoli** gates, 7 of which have a negated control.

<p align="center">
    <img src="https://github.com/LauraMDonaire/Review-Quantum-Comparators-2009-2021/blob/main/Full%20Comparators/Xia%20et%20al.%202019/Xias%20Quantum%20Full%20Comparator%20(n%3D4).png" alt="Xia et al. proposed 4-bit comparator" width="500"/>
</p>
<p align="center">
    <b>Figure 4: 4-bit Full Comparator proposed by Xia et al. (2019)</b>
</p>

The last full comparator they propose is the 8-bit one (see **Figure 6**). This comparator is made up of 31 **CNOT** gates and 17 **Toffoli** gates, 15 of which have a negated control.

<p align="center">
    <img src="https://github.com/LauraMDonaire/Review-Quantum-Comparators-2009-2021/blob/main/Full%20Comparators/Xia%20et%20al.%202019/Xias%20Quantum%20Full%20Comparator%20(n%3D8).png" alt="Xia et al. proposed 8-bit comparator" width="500"/>
</p>
<p align="center">
    <b>Figure 6: 8-bit Full Comparator proposed by Xia et al. (2019)</b>
</p>
  
The metrics of this circuits can be seen in **Table 1**. 
- **IBM Quantum Platform**: [View Circuit (n=8) on IBM Quantum Platform](https://quantum.ibm.com/composer/files/new?initial=N4IgdghgtgpiBcIAaBLCACGAXdEA2AdOgEwAMAjAJzoAUYAvABwCU6AYgMLoC06AygAkAggCUAogBEQAGhABHCAGcoCEAHkACmIByARSF8AsiQKkA3AB0wKMAGM8AVwAmMdBfkw8KAEbkCN23dLMDkAJxgAc3Q5UgBtAGYAXWCwyOjyWOJkq1SouWJM7JDwvPjClJLogBZynMq5AFZa4rS5ADZm3OiAdgSiq1tK21jyRn6wAAtouNIiqZiRovDFbGnm%2BYzZ4I3F7eiCrat5gvI56LLDyfPdo%2BrYy-ma073G%2B7PX59v2t5eOz6u5L0Hj0bmBlqtAc1bAAPNanaRrS4w9KLBFyTZFZH5VH7H4DWFyMrw65IglPRJomqk6JNYmvanfOkdBm9OlAzEEjFouL-bwQUKhFAwUKIilwsULLJorkoukHCUnCUXJU4uRUiXktFNWZa1XMiV-CXstGso1QrEzCU8q1QgmK6WgvkCoUihY68XcwoO93o1XytH2kkqunqymq7US2kGt5ow0mmMgtnNTl4uwWr0on0Zf5YokK0Epy5OwXC0WeulxKWZiXZ-M%2BwOEhONkNNzU0ptR2NNuMgn2m%2BNZYJ21O2LG1gNNxXBLFt5tFYdF-kl12W8s2qu%2BrN%2Byeq5VovNhn2ziO6pnd1XGxNmwdWAnK6dYht7645gmdu7-O%2Bp4sussetYbjKvpyjudLPnOh4auGHZ6ueSZ9heyZ3EiuaqqGH4ctEPYfPOyFFD%2BpZujaFYZpuNbbvWu5NgeeFhnSJ7tmePrYZekJJjeYBviOM7QT6UbTgS-ZYQW7aLs6hGrv%2BkrkVuIGUWB1Foa2vGRrBzGIQh7G4d8KFcUx0avleA7afqwQESuTbWp6gFNuOuLySqPo0Wqyn0TB%2BldvBZpaUOvaYliLFNr0HGCd%2BS6-kRa7WTJ5FyfmClOUpR4qae0bqV58Y%2Bbewm6YxaUGSZYXiRZPpWQBMUOnFE4JcGUHJW5fFqQV8aade2kRg%2BZIpXlAlGcJn6ifh4USZZqqVhVsp1vFjm1ZBdGqY1Hn9WarXGb5Lm5RBtEYb1jKqQNG1DcVf4LCRNmyVN1UzfuSVQQ1%2B35Z5K3eW1633gMj5UYlhk4fNb1FcuJ1ldJ3qxZduI1TdLb1QtD1dulz2Za92XYptdmo9Nu2znm63ymZw0lcR64TcB4PYpDL51XdsOpfDzV%2BUja0oxinXlaDlWYVt5PaSzVjmUDY2kUB6P%2BhD12U3NGG6otj3LS1L1M2mBKSadxO7Q2ta7ej4348dkVSeN7OTRODk3d9VPzdLcM5fTkKrSCHHpiRDLo7zdjDnFu3Oe97tS3hu3vvSnPYaZ%2BJ9XbR2A-rqvRUbpMm9NZuzdtLn3bTNtPfLjMO0UsBKA44SijwAB86DDJceeKAXriqyXZegpX1flXXwwcY3hdkS3fTBO3Ne1l3VS5zA%2Bcd-KXcNEPI814qXdtJPVcd8qXfdPPTdzl3Yw98PC81%2BqXeUKvHfkl35AV9va8Rif-y93lJ9t%2BfHf6ifSRb1Py0n4Pr8735J8T1-a%2BmhPnPf%2BHdgqJBPivYIAB6KB6AAACtgAD2jgoBgEUOge40hSBYJwdgvBuCCH4KIQQ8g0hSHkLIZQihxBpDxGkFUeh0gGjSDaNIbobDpCMGkJQMh2DyDkPITQ8gdDyAMPIMw8RZDWHkHYaMMhPCqDSDIEo0hxAaHEDoRopRDDiDMOIKw4g7DDFKK4cQHh8RsHxFIfEGh8Q6HxAYfEZh8RWHxHYfELh8RzE8KqNgqopCqg0KqHQ4J9CGFVGYVUVhVR2ExPoVwqoPCGjYIaKQ1JTCaENDoQ0BhDRmF5KYawho7CGhcNKUwnhbRsFtFITUlhtSGn1KaXUtoNC2h0LaAwtozC2isLaOwtoXC2g8O6Ng7opDug0O6HQ7oDDujMO6Kw7o7DuhcO6DwxgswrAyBAC4RQgwUAAAcsAoEQWAVQIAAC%2BQA)


## Metrics

The following table summarizes the quantum cost metrics for the half-comparator circuits, evaluated for various values of $n$. Please note that these metrics are based on general implementations of the quantum gates used in each circuit. For accurate reproduction of these results, understanding the specific context and details of the gate implementations is essential. Feel free to reach out to me for any questions or further clarification regarding these implementations.

| Circuit                | Size of n        | Quantum Cost | Delay | T-count | T-depth | Ancillary Inputs |
|------------------------|------------------|--------------|-------|---------|---------|------------------|
| Al-Rabadi et al. (2009)| 2                | 44           | 35    | 42      | 18      | 6                |
| Xia et al. (2019)      | 1                | 14           | 14    | 14      | 6       | 2                |
| Xia et al. (2019)      | 2                | 38           | 35    | 35      | 15      | 2                |
| Xia et al. (2019)      | 3                | 56           | 49    | 49      | 21      | 2                |
| Xia et al. (2019)      | 4                | 74           | 63    | 63      | 27      | 2                |
| Xia et al. (2019)      | 8                | 146          | 119   | 119     | 51      | 2                |

**Table 1: Metrics for Full Comparators studied for specific values of n.**
