## Description

<div><p>You are given two qubits which are guaranteed to be in one of the Bell states:</p><ul><li> <img align="middle" class="tex-formula" src="./29369/file/0DeznrYc.png" style="max-width: 100.0%;max-height: 100.0%;"></li><li> <img align="middle" class="tex-formula" src="./29369/file/iTsYAiuP.png" style="max-width: 100.0%;max-height: 100.0%;"></li><li> <img align="middle" class="tex-formula" src="./29369/file/mAUMQwEK.png" style="max-width: 100.0%;max-height: 100.0%;"></li><li> <img align="middle" class="tex-formula" src="./29369/file/seDx9hRK.png" style="max-width: 100.0%;max-height: 100.0%;"></li></ul><p>Your task is to perform necessary operations and measurements to figure out which state it was and to return the index of that state (0 for <img align="middle" class="tex-formula" src="./29369/file/guLUlP86.png" style="max-width: 100.0%;max-height: 100.0%;">, 1 for <img align="middle" class="tex-formula" src="./29369/file/vzeWlYct.png" style="max-width: 100.0%;max-height: 100.0%;"> etc.). The state of the qubits after the operations does not matter.</p></div><div class="input-specification"><p>You have to implement an operation which takes an array of two qubits as an input and returns an integer. </p><p>Your code should have the following signature:</p><pre class="verbatim">namespace Solution {
    open Microsoft.Quantum.Primitive;
    open Microsoft.Quantum.Canon;

    operation Solve (qs : Qubit[]) : Int
    {
        body
        {
            // your code here
        }
    }
}</pre></div>

## Input

<p>You have to implement an operation which takes an array of two qubits as an input and returns an integer. </p><p>Your code should have the following signature:</p><pre class="verbatim">namespace Solution {
    open Microsoft.Quantum.Primitive;
    open Microsoft.Quantum.Canon;

    operation Solve (qs : Qubit[]) : Int
    {
        body
        {
            // your code here
        }
    }
}</pre>
