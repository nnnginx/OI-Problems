## Description

<div><p>Implement a quantum oracle on $N$ qubits which checks whether the input bit string is balanced, i.e., whether it has exactly $\frac{N}{2}$ zeros and $\frac{N}{2}$ ones in it. </p><p>Your operation should take the following inputs:</p><ul> <li> an array of $N \le 10$ qubits "inputs" in an arbitrary state. $N$ will be an even number. </li><li> a qubit "output" in an arbitrary state. </li></ul><p>Your operation should perform a unitary transformation on those qubits that can be described by its effect on the basis states: if "inputs" is in the basis state $|x\rangle$ and "output" is in the basis state $|y\rangle$, the result of applying the operation should be $|x\rangle|y \oplus f(x)\rangle$, where $f(x) = 1$ if the bit string $x$ has the same number of zeros and ones in it, and $0$ otherwise.</p><p>For example, if the qubits passed to your operation are in the state $\frac{1}{\sqrt{2}}(|01\rangle + |00\rangle)_x \otimes |0\rangle_y$, the state of the system after applying the operation should be $\frac{1}{\sqrt{2}}(|01\rangle_x\otimes |1\rangle_y + |00\rangle_x |0\rangle_y)$.</p><p>Your code should have the following signature (note that your operation should have Adjoint and Controlled variants defined for it; <span class="tex-font-style-tt">is Adj+Ctl</span> in the operation signature will generate them automatically based on your code):</p><pre class="verbatim">namespace Solution {
    open Microsoft.Quantum.Intrinsic;

    operation Solve (inputs : Qubit[], output : Qubit) : Unit is Adj+Ctl {
        // your code here
    }
}</pre><p>Your code is not allowed to use measurements or arbitrary rotation gates. This operation can be implemented using just the X gate and its controlled variants (possibly with multiple qubits as controls).</p></div>
