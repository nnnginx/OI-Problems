## Description

<div><p>Implement a quantum oracle on <span class="tex-span"><i>N</i></span> qubits which implements a function <span class="tex-span"><i>f</i>(<i>x</i>) = <i>x</i><sub class="lower-index"><i>k</i></sub></span>, i.e. the value of the function is the value of the <span class="tex-span"><i>k</i></span>-th qubit.</p><p>For an explanation on how the quantum oracles work, see <a href="https://codeforces.com/blog/entry/60319">the tutorial blog post</a>.</p></div><div class="input-specification"><p>You have to implement an operation which takes the following inputs:</p><ul><li> an array of qubits <span class="tex-span"><i>x</i></span> (input register),</li><li> a qubit <span class="tex-span"><i>y</i></span> (output qubit),</li><li> 0-based index of the qubit from input register <span class="tex-span"><i>K</i></span> (<img align="middle" class="tex-formula" src="./29371/file/BqLwFAcB.png" style="max-width: 100.0%;max-height: 100.0%;">).</li></ul><p>The operation doesn't have an output; the "output" of your solution is the state in which it left the qubits.</p><p>Your code should have the following signature:</p><pre class="verbatim">namespace Solution {
    open Microsoft.Quantum.Primitive;
    open Microsoft.Quantum.Canon;

    operation Solve (x : Qubit[], y : Qubit, k : Int) : ()
    {
        body
        {
            // your code here
        }
    }
}</pre></div>

## Input

<p>You have to implement an operation which takes the following inputs:</p><ul><li> an array of qubits <span class="tex-span"><i>x</i></span> (input register),</li><li> a qubit <span class="tex-span"><i>y</i></span> (output qubit),</li><li> 0-based index of the qubit from input register <span class="tex-span"><i>K</i></span> (<img align="middle" class="tex-formula" src="./29371/file/BqLwFAcB.png" style="max-width: 100.0%;max-height: 100.0%;">).</li></ul><p>The operation doesn't have an output; the "output" of your solution is the state in which it left the qubits.</p><p>Your code should have the following signature:</p><pre class="verbatim">namespace Solution {
    open Microsoft.Quantum.Primitive;
    open Microsoft.Quantum.Canon;

    operation Solve (x : Qubit[], y : Qubit, k : Int) : ()
    {
        body
        {
            // your code here
        }
    }
}</pre>
