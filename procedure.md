# Procedure

The agent performs resource estimation using BenchQ for CO at multiple bond lengths while keeping all other parameters fixed.

## Workflow

1. For each bond length, load the corresponding FCIDUMP file.
2. Construct the second-quantized electronic Hamiltonian.
3. Apply double-factorized Hamiltonian compression.
4. Run QPE-based resource estimation using BenchQ.
5. Compute:
   - Toffoli gate count
   - Logical qubit count
   - Hamiltonian norms and sparsity metrics
6. Apply the physical cost model using Litinski-style magic state factories.
7. Extract:
   - Physical qubit count
   - Code distance
   - Runtime
   - Logical error rate

## BenchQ APIs used

- `benchq.problem_embeddings.qpe.get_double_factorized_qpe_toffoli_and_qubit_cost`
- FCIDUMP-based Hamiltonian construction pipeline within BenchQ

## Tools and execution

- BenchQ (primary estimator)
- Python execution environment
- FCIDUMP input files
