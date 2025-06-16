## Description

<div><p>You are given two qubits in state $|00 \rangle$. Your task is to create the following state on them:</p><p>$$\frac{1}{\sqrt{3}} \big( |00 \rangle + |01 \rangle + |10 \rangle)$$</p><p>You have to implement an operation which takes an array of 2 qubits as an input and has no output. The "output" of your solution is the state in which it left the input qubits.</p><p>Your code should have the following signature:</p><pre class="verbatim">namespace Solution {
    open Microsoft.Quantum.Primitive;
    open Microsoft.Quantum.Canon;

    operation Solve (qs : Qubit[]) : Unit {
        // your code here
    }
}</pre></div>
