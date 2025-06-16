## Description

<div><p>You are given 2 qubits which are guaranteed to be in one of the four orthogonal states:</p><ul><li> <img align="middle" class="tex-formula" src="./29381/file/rXrlP6Y5.png" style="max-width: 100.0%;max-height: 100.0%;"></li><li> <img align="middle" class="tex-formula" src="./29381/file/tjWWUeBN.png" style="max-width: 100.0%;max-height: 100.0%;"></li><li> <img align="middle" class="tex-formula" src="./29381/file/bG5nNFzW.png" style="max-width: 100.0%;max-height: 100.0%;"></li><li> <img align="middle" class="tex-formula" src="./29381/file/oRIi9vrH.png" style="max-width: 100.0%;max-height: 100.0%;"></li></ul><p>Your task is to perform necessary operations and measurements to figure out which state it was and to return the index of that state (0 for <img align="middle" class="tex-formula" src="./29381/file/Rl2hg31v.png" style="max-width: 100.0%;max-height: 100.0%;">, 1 for <img align="middle" class="tex-formula" src="./29381/file/9RDBZ9Ys.png" style="max-width: 100.0%;max-height: 100.0%;"> etc.). The state of the qubits after the operations does not matter.</p><p>You have to implement an operation which takes an array of 2 qubits as an input and returns an integer. </p><p>Your code should have the following signature:</p><pre class="verbatim">namespace Solution {
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
