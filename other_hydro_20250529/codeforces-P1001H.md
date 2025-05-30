## Description

<div><p>Implement a quantum oracle on <span class="tex-span"><i>N</i></span> qubits which implements the following function: <img align="middle" class="tex-formula" src="./29372/file/gCAs7Vm8.png" style="max-width: 100.0%;max-height: 100.0%;">, i.e., the value of the function is 1 if <span class="tex-span"><i>x</i></span> has odd number of 1s, and 0 otherwise.</p></div><div class="input-specification"><p>You have to implement an operation which takes the following inputs:</p><ul><li> an array of qubits <span class="tex-span"><i>x</i></span> (input register),</li><li> a qubit <span class="tex-span"><i>y</i></span> (output qubit).</li></ul><p>The operation doesn't have an output; the "output" of your solution is the state in which it left the qubits.</p><p>Your code should have the following signature:</p><pre class="verbatim">namespace Solution {
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

## Input

<p>You have to implement an operation which takes the following inputs:</p><ul><li> an array of qubits <span class="tex-span"><i>x</i></span> (input register),</li><li> a qubit <span class="tex-span"><i>y</i></span> (output qubit).</li></ul><p>The operation doesn't have an output; the "output" of your solution is the state in which it left the qubits.</p><p>Your code should have the following signature:</p><pre class="verbatim">namespace Solution {
    open Microsoft.Quantum.Primitive;
    open Microsoft.Quantum.Canon;

    operation Solve (x : Qubit[], y : Qubit) : ()
    {
        body
        {
            // your code here
        }
    }
}</pre>
