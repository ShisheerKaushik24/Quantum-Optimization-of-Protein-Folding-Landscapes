# Determining the conformation of a protein that corresponds to its lowest possible energy state

In the Qiskit implementation of the **protein folding problem**, each **amino acid** is represented by **two qubits**, and each qubit can take on one of *three states* corresponding to the three possible conformations for that amino acid. So in general, the total number of qubits required for a protein with **N** amino acids is approximately **2N** for a *simplified representation* and **4N** for a more *detailed representation*. Therefore, the total number of qubits required is:

```bash
total_qubits = 2 * num_amino_acids # For simplified representation
total_qubits = 4 * num_amino_acids # For detailed representation
``` 
<div class="html">

For instance, if you define the `main_chain` variable to be <span style="color:red">"APRLRFYHIL"</span> and the `side_chains` variable to be **[""] * 10**, then the total number of amino acids in the protein is 10, and the total number of qubits required is:

</div>

```bash
total_qubits = 2 * 10 = 20 # For simplified representation
total_qubits = 4 * 10 = 40 # For detailed representation
```
