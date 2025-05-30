## Description

<div><p>You are given <span class="tex-span"><i>N</i> = 2<sup class="upper-index"><i>k</i></sup></span> qubits (<span class="tex-span">0 ≤ <i>k</i> ≤ 4</span>) in zero state <img align="middle" class="tex-formula" src="./29378/file/QUxhslQt.png" style="max-width: 100.0%;max-height: 100.0%;">. Your task is to create a generalized <a href="https://en.wikipedia.org/wiki/W_state">W state</a> on them. Generalized W state is an equal superposition of all basis states on <span class="tex-span"><i>N</i></span> qubits that have Hamming weight equal to 1:</p><center class="tex-equation"><img align="middle" class="tex-formula" src="./29378/file/W2UuiPYQ.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>For example, for <span class="tex-span"><i>N</i> = 1</span>, <img align="middle" class="tex-formula" src="./29378/file/tUt3aTIW.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>You have to implement an operation which takes an array of <span class="tex-span"><i>N</i></span> qubits as an input and has no output. The "output" of the operation is the state in which it leaves the qubits.</p><p>Your code should have the following signature:</p><pre class="verbatim">namespace Solution {
    open Microsoft.Quantum.Primitive;
    open Microsoft.Quantum.Canon;

    operation Solve (qs : Qubit[]) : ()
    {
        body
        {
            // your code here
        }
    }
}</pre></div>
