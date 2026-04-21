# Findings

The agent successfully performed resource estimation for CO across bond lengths from 0.83 Å to 1.33 Å using a consistent BenchQ workflow.

## Key results

- Toffoli count decreases from ~466M to ~436M as bond length increases
- Logical qubits remain mostly constant (360 → 366)
- Physical qubits increase slightly when logical qubits increase
- Total runtime decreases steadily across the scan
- Logical error rate remains stable (~1.8e-4 to ~1.9e-4)
