## Description

<div><p>You are given an operation that implements a two-qubit unitary transformation: either the CNOT gate with the first qubit as control and the second qubit as target (CNOT$_{12}$), or the CNOT gate with the second qubit as control and the first qubit as target (CNOT$_{21}$). The operation will have Adjoint and Controlled variants defined.</p><p>Your task is to perform necessary operations and measurements to figure out which unitary it was and to return 0 if it was the CNOT$_{12}$ gate or 1 if it was the CNOT$_{21}$ gate. </p><p>You are allowed to apply the given operation and its adjoint/controlled variants <span class="tex-font-style-bf">exactly once</span>.</p><p>You have to implement an operation which takes a two-qubit operation <span class="tex-font-style-tt">unitary</span> as an input and returns an integer. The operation <span class="tex-font-style-tt">unitary</span> will accept an array of qubits as input, but it will fail if the array is empty or has one or more than two qubits. Your code should have the following signature:</p><pre class="verbatim">namespace Solution {
    open Microsoft.Quantum.Intrinsic;

    operation Solve (unitary : (Qubit[] =&gt; Unit is Adj+Ctl)) : Int {
        // your code here
    }
}</pre></div>
