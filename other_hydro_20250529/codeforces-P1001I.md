## Description

<div><p>You are given a quantum oracle - an operation on <span class="tex-span"><i>N</i> + 1</span> qubits which implements a function <img align="middle" class="tex-formula" src="./29373/file/LX1Uq4Ar.png" style="max-width: 100.0%;max-height: 100.0%;">. You are guaranteed that the function <span class="tex-span"><i>f</i></span> implemented by the oracle is either constant (returns 0 on all inputs or 1 on all inputs) or balanced (returns 0 on exactly one half of the input domain and 1 on the other half).</p><p>There are only two possible constant functions: <span class="tex-span"><i>f</i>(<i>x</i>) = 0</span> and <span class="tex-span"><i>f</i>(<i>x</i>) = 1</span>. The functions implemented by oracles in the two previous problems (<span class="tex-span"><i>f</i>(<i>x</i>) = <i>x</i><sub class="lower-index"><i>k</i></sub></span> and <img align="middle" class="tex-formula" src="./29373/file/HQqSCo6C.png" style="max-width: 100.0%;max-height: 100.0%;">) are examples of balanced functions.</p><p>Your task is to figure out whether the function given by the oracle is constant. Your code is allowed to call the given oracle only once.</p></div><div class="input-specification"><p>You have to implement an operation which takes the following inputs:</p><ul><li> an integer <span class="tex-span"><i>N</i></span> - the number of qubits in the oracle input,</li><li> an oracle <span class="tex-span"><i>Uf</i></span>, implemented as an operation with signature <span class="tex-font-style-tt">((Qubit[], Qubit) =&gt; ())</span>, i.e., an operation which takes as input an array of qubits and an output qubit and has no output.</li></ul><p>The return of your operation is a Boolean value: true if the oracle implements a constant function and false otherwise.</p><p>Your code should have the following signature:</p><pre class="verbatim">namespace Solution {
    open Microsoft.Quantum.Primitive;
    open Microsoft.Quantum.Canon;

    operation Solve (N : Int, Uf : ((Qubit[], Qubit) =&gt; ())) : Bool
    {
        body
        {
            // your code here
        }
    }
}</pre></div>

## Input

<p>You have to implement an operation which takes the following inputs:</p><ul><li> an integer <span class="tex-span"><i>N</i></span> - the number of qubits in the oracle input,</li><li> an oracle <span class="tex-span"><i>Uf</i></span>, implemented as an operation with signature <span class="tex-font-style-tt">((Qubit[], Qubit) =&gt; ())</span>, i.e., an operation which takes as input an array of qubits and an output qubit and has no output.</li></ul><p>The return of your operation is a Boolean value: true if the oracle implements a constant function and false otherwise.</p><p>Your code should have the following signature:</p><pre class="verbatim">namespace Solution {
    open Microsoft.Quantum.Primitive;
    open Microsoft.Quantum.Canon;

    operation Solve (N : Int, Uf : ((Qubit[], Qubit) =&gt; ())) : Bool
    {
        body
        {
            // your code here
        }
    }
}</pre>
