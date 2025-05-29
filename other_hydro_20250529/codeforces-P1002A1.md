## Description

<div><p>You are given <span class="tex-span"><i>N</i></span> qubits (<span class="tex-span">1 ≤ <i>N</i> ≤ 8</span>) in zero state <img align="middle" class="tex-formula" src="./29375/file/sTWzLgk6.png" style="max-width: 100.0%;max-height: 100.0%;">. </p><p>Your task is to generate an equal superposition of all <span class="tex-span">2<sup class="upper-index"><i>N</i></sup></span> basis vectors on <span class="tex-span"><i>N</i></span> qubits:</p><center class="tex-equation"><img align="middle" class="tex-formula" src="./29375/file/QDerXfeV.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>For example,</p><ul><li> for <span class="tex-span"><i>N</i> = 1</span>, the required state is simply <img align="middle" class="tex-formula" src="./29375/file/nx43Fwkt.png" style="max-width: 100.0%;max-height: 100.0%;">,</li><li> for <span class="tex-span"><i>N</i> = 2</span>, the required state is <img align="middle" class="tex-formula" src="./29375/file/LzyHpIMx.png" style="max-width: 100.0%;max-height: 100.0%;">. </li></ul><p>You have to implement an operation which takes an array of <span class="tex-span"><i>N</i></span> qubits as an input and has no output. The "output" of the operation is the state in which it leaves the qubits.</p><p>Your code should have the following signature:</p><pre class="verbatim">namespace Solution {
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
