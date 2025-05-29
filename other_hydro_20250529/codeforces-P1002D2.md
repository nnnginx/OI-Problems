## Description

<div><p>Implement a quantum oracle on <span class="tex-span"><i>N</i></span> qubits which implements the following function: </p><center class="tex-equation"><img align="middle" class="tex-formula" src="./29386/file/WJ7pGqKi.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>Here <img align="middle" class="tex-formula" src="./29386/file/Jgo38N0m.png" style="max-width: 100.0%;max-height: 100.0%;"> (a vector of <span class="tex-span"><i>N</i></span> integers, each of which can be 0 or 1), and <img align="middle" class="tex-formula" src="./29386/file/SiOqnz3F.png" style="max-width: 100.0%;max-height: 100.0%;"> is a vector of <span class="tex-span"><i>N</i></span> 1s.</p><p>For an explanation on how this type of quantum oracles works, see <a href="https://codeforces.com/blog/entry/60319">Introduction to quantum oracles</a>.</p><p>You have to implement an operation which takes the following inputs:</p><ul><li> an array of <span class="tex-span"><i>N</i></span> qubits <span class="tex-span"><i>x</i></span> in arbitrary state (input register), <span class="tex-span">1 ≤ <i>N</i> ≤ 8</span>,</li><li> a qubit <span class="tex-span"><i>y</i></span> in arbitrary state (output qubit),</li><li> an array of <span class="tex-span"><i>N</i></span> integers <span class="tex-span"><i>b</i></span>, representing the vector <img align="middle" class="tex-formula" src="./29386/file/iMj57rgG.png" style="max-width: 100.0%;max-height: 100.0%;">. Each element of <span class="tex-span"><i>b</i></span> will be 0 or 1.</li></ul><p>The operation doesn't have an output; its "output" is the state in which it leaves the qubits.</p><p>Your code should have the following signature:</p><pre class="verbatim">namespace Solution {
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
