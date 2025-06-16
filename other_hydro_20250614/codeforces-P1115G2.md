## Description

<div><p>Implement a quantum oracle on $N$ qubits which implements the following function: $$f(\vec{x}) = x_0 \vee x_1 \vee \dotsb \vee x_{N-1}$$</p><p>You have to implement an operation which takes the following inputs:</p><ul><li> an array of $N$ ($1 \le N \le 8$) qubits $x$ in an arbitrary state (input register),</li><li> a qubit $y$ in an arbitrary state (output qubit),</li></ul><p>and performs a transformation $|x\rangle|y\rangle \rightarrow |x\rangle|y \oplus f(x)\rangle$. The operation doesn't have an output; its "output" is the state in which it leaves the qubits.</p><p>Your code should have the following signature:</p><pre class="verbatim">namespace Solution {
    open Microsoft.Quantum.Primitive;
    open Microsoft.Quantum.Canon;

    operation Solve (x : Qubit[], y : Qubit) : Unit {
        body (...) {
            // your code here
        }
        adjoint auto;
    }
}</pre></div>
