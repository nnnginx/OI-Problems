## Description

<div><p>You are given <span class="tex-span"><i>N</i></span> qubits (<span class="tex-span">1 ≤ <i>N</i> ≤ 8</span>) in zero state <img align="middle" class="tex-formula" src="./29367/file/b7Tlaye0.png" style="max-width: 100.0%;max-height: 100.0%;">. Your task is to create Greenberger–Horne–Zeilinger (GHZ) state on them:</p><center class="tex-equation"><img align="middle" class="tex-formula" src="./29367/file/pGaYrnXF.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>Note that for <span class="tex-span"><i>N</i> = 1</span> and <span class="tex-span"><i>N</i> = 2</span> GHZ state becomes states <img align="middle" class="tex-formula" src="./29367/file/bGZiUknv.png" style="max-width: 100.0%;max-height: 100.0%;"> and <img align="middle" class="tex-formula" src="./29367/file/algvjk7E.png" style="max-width: 100.0%;max-height: 100.0%;"> from the previous tasks, respectively.</p></div><div class="input-specification"><p>You have to implement an operation which takes an array of <span class="tex-span"><i>N</i></span> qubits as an input and has no output. The "output" of your solution is the state in which it left the input qubits.</p><p>Your code should have the following signature:</p><pre class="verbatim">namespace Solution {
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

## Input

<p>You have to implement an operation which takes an array of <span class="tex-span"><i>N</i></span> qubits as an input and has no output. The "output" of your solution is the state in which it left the input qubits.</p><p>Your code should have the following signature:</p><pre class="verbatim">namespace Solution {
    open Microsoft.Quantum.Primitive;
    open Microsoft.Quantum.Canon;

    operation Solve (qs : Qubit[]) : ()
    {
        body
        {
            // your code here
        }
    }
}</pre>
