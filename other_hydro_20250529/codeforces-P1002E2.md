## Description

<div><p>You are given a quantum oracle - an operation on <span class="tex-span"><i>N</i> + 1</span> qubits which implements a function <img align="middle" class="tex-formula" src="./29389/file/6UfJy5DU.png" style="max-width: 100.0%;max-height: 100.0%;">. You are guaranteed that the function <span class="tex-span"><i>f</i></span> implemented by the oracle can be represented in the following form (oracle from problem D2):</p><center class="tex-equation"><img align="middle" class="tex-formula" src="./29389/file/MVOaAuIs.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>Here <img align="middle" class="tex-formula" src="./29389/file/wOFVxxsj.png" style="max-width: 100.0%;max-height: 100.0%;"> (a vector of <span class="tex-span"><i>N</i></span> integers, each of which can be 0 or 1), and <img align="middle" class="tex-formula" src="./29389/file/H4KuVHfo.png" style="max-width: 100.0%;max-height: 100.0%;"> is a vector of <span class="tex-span"><i>N</i></span> 1s.</p><p>Your task is to reconstruct the array <img align="middle" class="tex-formula" src="./29389/file/tPEWouA7.png" style="max-width: 100.0%;max-height: 100.0%;"> which could produce the given oracle. Your code is allowed to call the given oracle only once.</p><p>You have to implement an operation which takes the following inputs:</p><ul><li> an integer <span class="tex-span"><i>N</i></span> - the number of qubits in the oracle input (<span class="tex-span">1 ≤ <i>N</i> ≤ 8</span>),</li><li> an oracle <span class="tex-span"><i>Uf</i></span>, implemented as an operation with signature <span class="tex-font-style-tt">((Qubit[], Qubit) =&gt; ())</span>, i.e., an operation which takes as input an array of qubits and an output qubit and has no output.</li></ul><p>The return of your operation is an array of integers of length <span class="tex-span"><i>N</i></span>, each of them 0 or 1.</p><p>Note that in this problem we're comparing the oracle generated by your return to the oracle <span class="tex-span"><i>Uf</i></span>, instead of comparing your return to the (hidden) value of <img align="middle" class="tex-formula" src="./29389/file/IgWF9FU1.png" style="max-width: 100.0%;max-height: 100.0%;"> used to generate <span class="tex-span"><i>Uf</i></span>. This means that any kind of incorrect return results in "Runtime Error" verdict, as well as actual runtime errors like releasing qubits in non-zero state.</p><p>Your code should have the following signature:</p><pre class="verbatim">namespace Solution {
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
