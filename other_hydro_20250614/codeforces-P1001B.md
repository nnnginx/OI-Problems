## Description

<div><p>You are given two qubits in state <img align="middle" class="tex-formula" src="./29366/file/hxD3lJKv.png" style="max-width: 100.0%;max-height: 100.0%;"> and an integer <span class="tex-span"><i>index</i></span>. Your task is to create one of the <a href="https://en.wikipedia.org/wiki/Bell_state">Bell states</a> on them according to the <span class="tex-span"><i>index</i></span>:</p><ul><li> <img align="middle" class="tex-formula" src="./29366/file/yst6Dchz.png" style="max-width: 100.0%;max-height: 100.0%;"></li><li> <img align="middle" class="tex-formula" src="./29366/file/jR8cKzrw.png" style="max-width: 100.0%;max-height: 100.0%;"></li><li> <img align="middle" class="tex-formula" src="./29366/file/kIiMWCyX.png" style="max-width: 100.0%;max-height: 100.0%;"></li><li> <img align="middle" class="tex-formula" src="./29366/file/qMkMRFMe.png" style="max-width: 100.0%;max-height: 100.0%;"></li></ul></div><div class="input-specification"><p>You have to implement an operation which takes an array of 2 qubits and an integer as an input and has no output. The "output" of your solution is the state in which it left the input qubits.</p><p>Your code should have the following signature:</p><pre class="verbatim">namespace Solution {
    open Microsoft.Quantum.Primitive;
    open Microsoft.Quantum.Canon;

    operation Solve (qs : Qubit[], index : Int) : ()
    {
        body
        {
            // your code here
        }
    }
}</pre></div>

## Input

<p>You have to implement an operation which takes an array of 2 qubits and an integer as an input and has no output. The "output" of your solution is the state in which it left the input qubits.</p><p>Your code should have the following signature:</p><pre class="verbatim">namespace Solution {
    open Microsoft.Quantum.Primitive;
    open Microsoft.Quantum.Canon;

    operation Solve (qs : Qubit[], index : Int) : ()
    {
        body
        {
            // your code here
        }
    }
}</pre>
