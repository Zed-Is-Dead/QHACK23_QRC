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
Initial ambition was to fully implement at least one use case with Pennylane and IBM-Q system (e.g. ibm_nairobi or # ibmq_jakarta) and to assess the impact of noise on the performance of the QR tasks. Due to lack of time, this program is postponed. However, the current state of the project is in our opinion a good starting point for a demo/tutorial on this promising field of research.  

## Abstract

Quantum Reservoir Computing (QRC) is the combination of quantum computing and physical reservoir computing to harness complex quantum dynamics as a reservoir for real-time machine learning tasks [[1](https://arxiv.org/abs/1602.08159v2)]. The approach followed by QRC is to exploit the complexity of natural (disordered) quantum dynamics for information processing. The framework of QRC enables to universally emulate nonlinear dynamical systems including classical chaos [[2](https://arxiv.org/abs/2011.04890)]. One potential interest in the NISQ era is suggested by a recent result which states that quantum noise could be used to improve the performance
of QRC [[3](https://arxiv.org/abs/2301.06814v2)].

A variety of quantum systems have been proposed to be used as the quantum reservoir, including quantum annealers, quantum circuits, and spin chains. The fully connected transverse field Ising (FC-TFI) model is a specific type of quantum spin chain, where each spin interacts with every other spin in the chain. The interactions between the spins are described by a Hamiltonian, which also includes a transverse field. 

One advantage of using the FC-TFI model as the reservoir in QRC is that it has been shown to be a universal quantum computer, meaning that it can be used to implement any quantum computation. This means that the FC-TFI model has the potential to perform a wide range of machine learning tasks, from classification to regression to time-series prediction. Another key feature of the FC-TFI model is its ability to learn *nonlinear* functions which emulate a specific target output by training the *linear* readout weights of the reservoir states.

In this demo, we describe how to implement QRC techniques with [PennyLane](https://pennylane.ai/). Our quantum reservoir is comprised of interacting quantum-mechanical spin systems, which are subject to the dynamics governed by the Fully Connected Transverse Field Ising (FC-TFI) Hamiltonian. In QRC, the input data is encoded into orthogonal basis states, and the dynamics of the system is used emulate nonlinear functions. As a first application, we consider the task of learning temporal sequences, with the objective of (at least) reproducing the results obtained in a recent article [[4](https://arxiv.org/abs/2301.08796)].

We make use of Pennylane simulation devices and will extend selected examples as experiments on IBM-Q real hardware.

## References

[1]  K. Fujii, K. Nakajima, [Harnessing disordered quantum dynamics for machine learning](https://arxiv.org/abs/1602.08159v2), Phys. Rev. Applied 8, 024030 (2017)

[2]  K. Fujii, K. Nakajima, [Quantum reservoir computing: a reservoir approach toward quantum machine learning on near-term quantum devices](https://arxiv.org/abs/2011.04890), arXiv:2011.04890

[3] L. Domingo et al., [Taking advantage of noise in quantum reservoir computing](https://arxiv.org/abs/2301.06814v2), arXiv:2301.06814v2

[4] Z. Mlika et al., [User Trajectory Prediction in Mobile Wireless Networks Using Quantum Reservoir Computing](https://arxiv.org/abs/2301.08796), arXiv:2301.08796



