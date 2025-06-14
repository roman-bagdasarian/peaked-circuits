# BlueQubit Challenge, Yale University Quantum Hackathon 2025

![1745188181547](https://github.com/user-attachments/assets/52cdd191-4f64-4695-9af0-13e92330c4af)

# Challenge

Peaked Circuits are special quantum circuits in ```.qasm``` [format](https://en.wikipedia.org/wiki/OpenQASM) where each circuit sets up a single hidden bitstring with high probability.

For example, ```1001``` is the peak bitstring as it has a much higher probability to be measured.

<img width="1031" alt="image" src="https://github.com/user-attachments/assets/3eb1b25b-a9f5-4921-aeab-ecf6c2ae9f4b" />

The ```.qasm``` [file](https://github.com/roman-bagdasarian/yquantum/blob/main/circuits/P1_little_peak.qasm) preparing the state:

```
OPENQASM 2.0;
include "qelib1.inc";
qreg q[4];
x q[1];
x q[2];
ry(0.8*pi) q[0];
ry(0.8*pi) q[1];
ry(0.8*pi) q[2];
ry(0.8*pi) q[3];
```

# Peaked Circuits

**Peaked circuits** are quantum circuits with a non-uniform ```O(1)``` distribution of measurement outcomes.
They were introduced by Scott Aaronson [1] to achieve a verifiable quantum advantage that would take supercomputers septillion ```=10²⁵``` years to replicate.


# Installation

```pip install -r requirements.txt```

# References
- Scott Aaronson and Yuxuan Zhang. “On Verifiable Quantum Advantage with Peaked Circuit Sampling.” *arXiv*, May 21, 2024. [arXiv:2404.14493](https://doi.org/10.48550/arXiv.2404.14493)
- Krishnageetha Karuppasamy, Varun Puram, Stevens Johnson, and Johnson P. Thomas. “A Comprehensive Review of Quantum Circuit Optimization: Current Trends and Future Directions.” *arXiv*, Jan. 2, 2025. [arXiv:2408.08941](https://doi.org/10.48550/arXiv.2408.08941)
- Xin-Chuan Wu, Marc Grau Davis, Frederic T. Chong, and Costin Iancu. “Reoptimization of Quantum Circuits via Hierarchical Synthesis.” In *2021 International Conference on Rebooting Computing (ICRC)*, Los Alamitos, CA, USA: IEEE, 2021, pp. 35–46. [IEEE Xplore](https://doi.org/10.1109/ICRC53822.2021.00016)
- J.-H. Bae, Paul M. Alsing, Doyeol Ahn, and Warner A. Miller. “Quantum Circuit Optimization Using Quantum Karnaugh Map.” *Scientific Reports*, vol. 10, no. 1, Sep. 24, 2020, article 15651. [doi:10.1038/s41598-020-72469-7](https://doi.org/10.1038/s41598-020-72469-7)
- John T. M. Campbell. “Bridging Relations between SVD in Tensor Networks and Common Matrix Operations in Quantum Information Theory.” *arXiv*, Feb. 4, 2024. [arXiv:2402.02517](https://doi.org/10.48550/arXiv.2402.02517)
