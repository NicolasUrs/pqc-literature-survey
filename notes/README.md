# Notes on Relevant Sources

## 1. Mosca (2018): Cybersecurity in an Era with Quantum Computers: Will We Be Ready?

The paper introduces three factors for assessing quantum security risks: the security shelf life of information, the migration time, and the time remaining until quantum computers can break current cryptographic systems. I use this model to explain the urgency of migrating to post-quantum cryptography and motivate the HNDL threat.

## 2. NIST IR 8547: Transition to Post-Quantum Cryptography Standards

The report identifies vulnerable cryptographic algorithms and describes the transition towards post-quantum alternatives. NIST recommends ML-KEM-768 as the default parameter set, providing a balance between security and performance. I use this recommendation to justify selecting ML-KEM-768 for my experimental environment.

## 3. RFC 10024: Post-Quantum Traditional (PQ/T) Hybrid Key Agreement Mechanisms for TLS 1.3

The RFC specifies hybrid key exchange mechanisms for TLS 1.3, including X25519MLKEM768, which combines classical X25519 with post-quantum ML-KEM-768. I use this specification as a technical reference for implementing and validating hybrid key exchange in my testbed.

## 4. Gidney (2025): How to Factor 2048-bit RSA Integers with Less Than a Million Noisy Qubits

The paper estimates that RSA-2048 could be factored in less than a week using fewer than one million noisy qubits, under specific hardware and error-rate assumptions. I use these estimates to illustrate the potential impact of quantum computing on current public-key cryptographic systems.

## 5. Paquin et al. (2020): Benchmarking Post-Quantum Cryptography in TLS

The authors build a testbed that controls link latency and packet loss to measure the impact of post-quantum algorithms on TLS connection establishment. I use their methodology as a reference for designing performance tests and comparing classical and hybrid post-quantum TLS connections.
