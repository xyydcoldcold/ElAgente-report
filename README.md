# BenchQ resource estimation case (El Agente)

This case demonstrates El Agente performing quantum resource estimation for a CO molecule across multiple bond lengths using BenchQ.

## Why this problem matters

Estimating ground-state energy using quantum phase estimation (QPE) is a central application of fault-tolerant quantum computing. However, practical feasibility depends on resource requirements such as logical qubits and non-Clifford gate counts (e.g., Toffoli gates), rather than just algorithmic correctness.

This task evaluates whether an agent can correctly execute a full workflow:
FCIDUMP → second-quantized Hamiltonian → double-factorized representation → QPE-based resource estimation → physical cost model.

It is a challenging problem because it requires consistent integration of quantum chemistry data, Hamiltonian representations, and fault-tolerant cost models under strict constraints where only geometry (bond length) is varied.