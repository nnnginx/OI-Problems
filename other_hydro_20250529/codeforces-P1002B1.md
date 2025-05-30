## Description

<div><p>You are given <span class="tex-span"><i>N</i></span> qubits (<span class="tex-span">2 ≤ <i>N</i> ≤ 8</span>) which are guaranteed to be in one of the two states:</p><ul> <li> <img align="middle" class="tex-formula" src="./29379/file/jendwgKI.png" style="max-width: 100.0%;max-height: 100.0%;"> state, or</li><li> <img align="middle" class="tex-formula" src="./29379/file/N3I4xQ0i.png" style="max-width: 100.0%;max-height: 100.0%;"> state. <p>Your task is to perform necessary operations and measurements to figure out which state it was and to return 0 if it was <img align="middle" class="tex-formula" src="./29379/file/UsqZQXna.png" style="max-width: 100.0%;max-height: 100.0%;"> state or 1 if it was W state. The state of the qubits after the operations does not matter.</p><p>You have to implement an operation which takes an array of <span class="tex-span"><i>N</i></span> qubits as an input and returns an integer. </p><p>Your code should have the following signature:</p><pre class="verbatim">namespace Solution {
    open Microsoft.Quantum.Primitive;
    open Microsoft.Quantum.Canon;

    operation Solve (qs : Qubit[]) : Int
    {
        body
        {
            // your code here
        }
    }
}</pre></li></ul></div>
