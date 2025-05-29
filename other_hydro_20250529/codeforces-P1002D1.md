## Description

<div><p>Implement a quantum oracle on <span class="tex-span"><i>N</i></span> qubits which implements the following function: <img align="middle" class="tex-formula" src="./29385/file/tbNy8fj2.png" style="max-width: 100.0%;max-height: 100.0%;">, where <img align="middle" class="tex-formula" src="./29385/file/ufcTEfgi.png" style="max-width: 100.0%;max-height: 100.0%;"> (a vector of <span class="tex-span"><i>N</i></span> integers, each of which can be 0 or 1).</p><p>For an explanation on how this type of quantum oracles works, see <a href="https://codeforces.com/blog/entry/60319">Introduction to quantum oracles</a>.</p><p>You have to implement an operation which takes the following inputs:</p><ul><li> an array of <span class="tex-span"><i>N</i></span> qubits <span class="tex-span"><i>x</i></span> in arbitrary state (input register), <span class="tex-span">1 ≤ <i>N</i> ≤ 8</span>,</li><li> a qubit <span class="tex-span"><i>y</i></span> in arbitrary state (output qubit),</li><li> an array of <span class="tex-span"><i>N</i></span> integers <span class="tex-span"><i>b</i></span>, representing the vector <img align="middle" class="tex-formula" src="./29385/file/uzdUIK6s.png" style="max-width: 100.0%;max-height: 100.0%;">. Each element of <span class="tex-span"><i>b</i></span> will be 0 or 1.</li></ul><p>The operation doesn't have an output; its "output" is the state in which it leaves the qubits.</p><p>Your code should have the following signature:</p><pre class="verbatim">namespace Solution {
    open Microsoft.Quantum.Primitive;
    open Microsoft.Quantum.Canon;

    operation Solve (x : Qubit[], y : Qubit, b : Int[]) : ()
    {
        body
        {
            // your code here
        }
    }
}</pre></div>
