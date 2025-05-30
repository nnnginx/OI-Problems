## Description

<div><p>You are given $N$ qubits in the state $|0...0 \rangle$, and an integer $parity \in \{0, 1\}$. Your task is to prepare an equal superposition of all basis states that have the given parity of the number of $1$s in their binary notation, i.e., the basis states that have an <span class="tex-font-style-it">even</span> number of $1$s if $parity = 0$ or the basis states that have an <span class="tex-font-style-it">odd</span> number of $1$s if $parity = 1$.</p><p>For example, for $N = 2$ the required state would be </p><ul> <li> $\frac{1}{\sqrt{2}} \big( |00 \rangle + |11 \rangle)$ if $parity = 0$. </li><li> $\frac{1}{\sqrt{2}} \big( |01 \rangle + |10 \rangle)$ if $parity = 1$. </li></ul><p>You are not allowed to use any gates except the Pauli gates (X, Y and Z), the Hadamard gate and the controlled versions of those (you are allowed to use multiple qubits as controls in the controlled versions of gates). However, you are allowed to use measurements.</p><p>You have to implement an operation which takes an array of $N$ qubits and an integer as an input and has no output. The "output" of your solution is the state in which it left the input qubits.</p><p>Your code should have the following signature:</p><pre class="verbatim">namespace Solution {
    open Microsoft.Quantum.Intrinsic;

    operation Solve (qs : Qubit[], parity : Int) : Unit {
        // your code here
    }
}</pre></div>
