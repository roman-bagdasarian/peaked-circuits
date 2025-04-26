# BlueQubit x Yale University Quantum Hackathon 2025

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
[1] Aaronson, Scott, and Yuxuan Zhang. ‘On Verifiable Quantum Advantage with Peaked Circuit Sampling’. arXiv, 21 May 2024. https://doi.org/10.48550/arXiv.2404.14493. <br/>
[2] Karuppasamy, Krishnageetha, Varun Puram, Stevens Johnson, and Johnson P. Thomas. ‘A Comprehensive Review of Quantum Circuit Optimization: Current Trends and Future Directions’. arXiv, 2 January 2025. https://doi.org/10.48550/arXiv.2408.08941. <br/>
[3] Wu, Xin-Chuan, Marc Grau Davis, Frederic T. Chong, and Costin Iancu. ‘Reoptimization of Quantum Circuits via Hierarchical Synthesis’. In 2021 International Conference on Rebooting Computing (ICRC), 35–46. Los Alamitos, CA, USA: IEEE, 2021. https://doi.org/10.1109/ICRC53822.2021.00016. <br/>
[4] Wu, Xin-Chuan, Marc Grau Davis, Frederic T. Chong, and Costin Iancu. ‘Reoptimization of Quantum Circuits via Hierarchical Synthesis’. In 2021 International Conference on Rebooting Computing (ICRC), 35–46. Los Alamitos, CA, USA: IEEE, 2021. https://doi.org/10.1109/ICRC53822.2021.00016. <br/>
[5] Bae, J.-H., Paul M. Alsing, Doyeol Ahn, and Warner A. Miller. ‘Quantum Circuit Optimization Using Quantum Karnaugh Map’. Scientific Reports 10, no. 1 (24 September 2020): 15651. https://doi.org/10.1038/s41598-020-72469-7. <br/>
[6] Campbell, John TM. ‘Bridging Relations between SVD in Tensor Networks and Common Matrix Operations in Quantum Information Theory’. arXiv, 4 February 2024. https://doi.org/10.48550/arXiv.2402.02517. <br/>
