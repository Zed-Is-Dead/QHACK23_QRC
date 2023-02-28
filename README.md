<div align="center">
  <a href="https://github.com/Zed-Is-Dead/"><img src="https://github.com/Zed-Is-Dead/QHACK23_QRC/blob/main/pics/quantum_computing_reservoir_01.jpg" height="800" width="800" /></a>
</div>

<div align="center">
  <h1> <a href="https://github.com/XanaduAI/QHack2023"> QHack2023 Open Hackathon </a> - <i> Patterns in the Ivy </i> Team Project </h1>
  <h2> Quantum Reservoir Computing with Pennylane </h2>
</div>


**Team name**: *Patterns in the Ivy*[^1]

**Topic**: Implementation of Quantum Reservoir Computing techniques with Pennylane

[^1]: Opeth song - MisterQ's favorite (Swedish) progmetal band 

---

## Motivation

The aim of this project is to *create a self-contained tutorial or demonstration of an idea from quantum computing* (see Paragraph "What hackathon project should my team do?" - [QHack2023/README.md at main · XanaduAI/QHack2023 (github.com)](https://github.com/XanaduAI/QHack2023/blob/main/README.md)).

### Disclaimer

This is a first introduction to the topic of *Quantum Reservoir Computing with Pennylane* and it will be followed by use case applications in subsequent developments.

## Abstract

Quantum Reservoir Computing (QRC) is the combination of quantum computing and physical reservoir computing to harness complex quantum dynamics as a reservoir for real-time machine learning tasks [[1](https://arxiv.org/abs/1602.08159v2)]. The approach followed by QRC is to exploit the complexity of natural (disordered) quantum dynamics for information processing. The framework of QRC enables to universally emulate nonlinear dynamical systems including classical chaos [[2](https://arxiv.org/abs/2011.04890)]. One potential interest in the NISQ era is suggested by a recent result which states that quantum noise could be used to improve the performance
of QRC [[3](https://arxiv.org/abs/2301.06814v2)].

In this demo, we describe how to implement QRC techniques with [PennyLane](https://pennylane.ai/). Our quantum reservoir is comprised of interacting quantum-mechanical spin systems, which are subject to the dynamics governed by the Fully Connected Transverse Field Ising (FC-TFI) Hamiltonian. As a first application, we consider the task of learning temporal sequences, with the objective of (at least) reproducing the results obtained in a recent article [[4](https://arxiv.org/abs/2301.08796)].

We make use of Pennylane simulation devices and will extend selected examples as experiments on IBM-Q real hardware.

## References

[1]  K. Fujii, K. Nakajima, [Harnessing disordered quantum dynamics for machine learning](https://arxiv.org/abs/1602.08159v2), Phys. Rev. Applied 8, 024030 (2017)

[2]  K. Fujii, K. Nakajima, [Quantum reservoir computing: a reservoir approach toward quantum machine learning on near-term quantum devices](https://arxiv.org/abs/2011.04890), arXiv:2011.04890

[3] L. Domingo et al., [Taking advantage of noise in quantum reservoir computing](https://arxiv.org/abs/2301.06814v2), arXiv:2301.06814v2

[4] Z. Mlika et al., [User Trajectory Prediction in Mobile Wireless Networks Using Quantum Reservoir Computing](https://arxiv.org/abs/2301.08796), arXiv:2301.08796



