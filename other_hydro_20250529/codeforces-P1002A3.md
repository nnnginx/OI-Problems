## Description

<div><p>You are given <span class="tex-span"><i>N</i></span> qubits (<span class="tex-span">1 ≤ <i>N</i> ≤ 8</span>) in zero state <img align="middle" class="tex-formula" src="./29377/file/DShYWOk8.png" style="max-width: 100.0%;max-height: 100.0%;">. You are also given two bitstrings <span class="tex-span"><i>bits</i>0</span> and <span class="tex-span"><i>bits</i>1</span> which describe two different basis states on <span class="tex-span"><i>N</i></span> qubits <img align="middle" class="tex-formula" src="./29377/file/x0m9WKgj.png" style="max-width: 100.0%;max-height: 100.0%;"> and <img align="middle" class="tex-formula" src="./29377/file/37DLwzIv.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>Your task is to generate a state which is an equal superposition of the given basis states:</p><center class="tex-equation"><img align="middle" class="tex-formula" src="./29377/file/Gy2NgUEO.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>You have to implement an operation which takes the following inputs:</p><ul><li> an array of qubits <span class="tex-span"><i>qs</i></span>,</li><li> two arrays of Boolean values <span class="tex-span"><i>bits</i>0</span> and <span class="tex-span"><i>bits</i>1</span> representing the basis states <img align="middle" class="tex-formula" src="./29377/file/OwSKcech.png" style="max-width: 100.0%;max-height: 100.0%;"> and <img align="middle" class="tex-formula" src="./29377/file/pGjNWqR3.png" style="max-width: 100.0%;max-height: 100.0%;">. These arrays will have the same length as the array of qubits. <span class="tex-span"><i>bits</i>0</span> and <span class="tex-span"><i>bits</i>1</span> will differ in at least one position.</li></ul><p>The operation doesn't have an output; its "output" is the state in which it leaves the qubits.</p><p>Your code should have the following signature:</p><pre class="verbatim">namespace Solution {
    open Microsoft.Quantum.Primitive;
    open Microsoft.Quantum.Canon;

    operation Solve (qs : Qubit[], bits0 : Bool[], bits1 : Bool[]) : ()
    {
        body
        {
            // your code here
        }
    }
}</pre></div>
