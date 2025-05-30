## Description

<div><p>You are given a quantum oracle - an operation on <span class="tex-span"><i>N</i> + 1</span> qubits which implements a function <img align="middle" class="tex-formula" src="./29388/file/8sl9c6Hl.png" style="max-width: 100.0%;max-height: 100.0%;">. You are guaranteed that the function <span class="tex-span"><i>f</i></span> implemented by the oracle is scalar product function (oracle from problem D1): </p><center class="tex-equation"><img align="middle" class="tex-formula" src="./29388/file/KYIWKfrf.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>Here <img align="middle" class="tex-formula" src="./29388/file/YpYa5MF8.png" style="max-width: 100.0%;max-height: 100.0%;"> (an array of <span class="tex-span"><i>N</i></span> integers, each of which can be 0 or 1). </p><p>Your task is to reconstruct the array <img align="middle" class="tex-formula" src="./29388/file/cQc8xQcp.png" style="max-width: 100.0%;max-height: 100.0%;">. Your code is allowed to call the given oracle only once.</p><p>You have to implement an operation which takes the following inputs:</p><ul><li> an integer <span class="tex-span"><i>N</i></span> - the number of qubits in the oracle input (<span class="tex-span">1 ≤ <i>N</i> ≤ 8</span>),</li><li> an oracle <span class="tex-span"><i>Uf</i></span>, implemented as an operation with signature <span class="tex-font-style-tt">((Qubit[], Qubit) =&gt; ())</span>, i.e., an operation which takes as input an array of qubits and an output qubit and has no output.</li></ul><p>The return of your operation is an array of integers of length <span class="tex-span"><i>N</i></span>, each of them 0 or 1.</p><p>Your code should have the following signature:</p><pre class="verbatim">namespace Solution {
    open Microsoft.Quantum.Primitive;
    open Microsoft.Quantum.Canon;

    operation Solve (N : Int, Uf : ((Qubit[], Qubit) =&gt; ())) : Int[]
    {
        body
        {
            // your code here
        }
    }
}</pre></div>
