## Description

<div><p>Implement a quantum oracle on $N$ qubits which checks whether the bits in the input vector $\vec{x}$ form a periodic bit string (i.e., implements the function $f(\vec{x}) = 1$ if $\vec{x}$ is periodic, and 0 otherwise). </p><p>A bit string of length $N$ is considered periodic with period $P$ ($1 \le P \le N - 1$) if for all $i \in [0, N - P - 1]$ $x_i = x_{i + P}$. Note that $P$ does not have to divide $N$ evenly; for example, bit string <span class="tex-font-style-tt">"01010"</span> is periodic with period $P = 2$.</p><p>You have to implement an operation which takes the following inputs:</p><ul><li> an array of $N$ ($2 \le N \le 7$) qubits $x$ in an arbitrary state (input register),</li><li> a qubit $y$ in an arbitrary state (output qubit),</li></ul><p>and performs a transformation $|x\rangle|y\rangle \rightarrow |x\rangle|y \oplus f(x)\rangle$. The operation doesn't have an output; its "output" is the state in which it leaves the qubits. Note that the input register $x$ has to remain unchanged after applying the operation.</p><p>Your code should have the following signature:</p><pre class="verbatim">namespace Solution {
    open Microsoft.Quantum.Primitive;
    open Microsoft.Quantum.Canon;

    operation Solve (x : Qubit[], y : Qubit) : Unit {
        body (...) {
            // your code here
        }
        adjoint auto;
    }
}</pre><p>Note: the operation has to have an adjoint specified for it; <span class="tex-font-style-tt">adjoint auto</span> means that the adjoint will be generated automatically. For details on adjoint, see <a href="https://docs.microsoft.com/en-us/quantum/language/file-structure#operation-definitions">Operation Definitions</a>.</p><p>You are not allowed to use measurements in your operation.</p></div>
