## Description

<div><p>Implement a quantum oracle on 3 qubits which implements a majority function. Majority function on 3-bit vectors is defined as follows: <img align="middle" class="tex-formula" src="./29387/file/CIs2ccxA.png" style="max-width: 100.0%;max-height: 100.0%;"> if vector <img align="middle" class="tex-formula" src="./29387/file/CDMdnqGn.png" style="max-width: 100.0%;max-height: 100.0%;"> has two or three 1s, and 0 if it has zero or one 1s.</p><p>For an explanation on how this type of quantum oracles works, see <a href="https://codeforces.com/blog/entry/60319">Introduction to quantum oracles</a>.</p><p>You have to implement an operation which takes the following inputs:</p><ul><li> an array of 3 qubits <span class="tex-span"><i>x</i></span> in arbitrary state (input register),</li><li> a qubit <span class="tex-span"><i>y</i></span> in arbitrary state (output qubit).</li></ul><p>The operation doesn't have an output; its "output" is the state in which it leaves the qubits.</p><p>Your code should have the following signature:</p><pre class="verbatim">namespace Solution {
    open Microsoft.Quantum.Primitive;
    open Microsoft.Quantum.Canon;

    operation Solve (x : Qubit[], y : Qubit) : ()
    {
        body
        {
            // your code here
        }
    }
}</pre></div>
