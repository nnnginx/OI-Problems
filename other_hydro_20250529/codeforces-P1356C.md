## Description

<div><p>You are given two qubits in state $|00 \rangle$. Your task is to prepare the following state on them:</p><p>$$\frac{1}{\sqrt{3}} \big( |01 \rangle + |10 \rangle + |11 \rangle)$$</p><p>This task is very similar to <a href="https://codeforces.com/contest/1116/problem/A1">problem A1 of the Winter 2019 contest</a>, but this time you are not allowed to use any gates except the Pauli gates (X, Y and Z), the Hadamard gate and the controlled versions of those. However, you are allowed to use measurements.</p><p>You have to implement an operation which takes an array of 2 qubits as an input and has no output. The "output" of your solution is the state in which it left the input qubits.</p><p>Your code should have the following signature:</p><pre class="verbatim">namespace Solution {
    open Microsoft.Quantum.Intrinsic;

    operation Solve (qs : Qubit[]) : Unit {
        // your code here
    }
}</pre></div>
