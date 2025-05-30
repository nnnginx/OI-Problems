## Description

<div><p>Implement a quantum oracle on $N$ qubits which checks whether the number of bits equal to 1 in the input vector $\vec{x}$ is divisible by 3 (i.e., implements the function $f(\vec{x}) = 1$ if the number of $x_i = 1$ in $\vec{x}$ is divisible by 3, and 0 otherwise).</p><p>You have to implement an operation which takes the following inputs:</p><ul><li> an array of $N$ ($1 \le N \le 9$) qubits $x$ in an arbitrary state (input register),</li><li> a qubit $y$ in an arbitrary state (output qubit),</li></ul><p>and performs a transformation $|x\rangle|y\rangle \rightarrow |x\rangle|y \oplus f(x)\rangle$. The operation doesn't have an output; its "output" is the state in which it leaves the qubits. Note that the input register $x$ has to remain unchanged after applying the operation.</p><p>Your code should have the following signature:</p><pre class="verbatim">namespace Solution {
    open Microsoft.Quantum.Primitive;
    open Microsoft.Quantum.Canon;

    operation Solve (x : Qubit[], y : Qubit) : Unit {
        body (...) {
            // your code here
        }
        adjoint auto;
    }
}</pre><p>Note: the operation has to have an adjoint specified for it; <span class="tex-font-style-tt">adjoint auto</span> means that the adjoint will be generated automatically. For details on adjoint, see <a href="https://docs.microsoft.com/en-us/quantum/language/file-structure#operation-declarations">Operation Declarations</a>.</p><p>You are not allowed to use measurements in your operation.</p></div>
