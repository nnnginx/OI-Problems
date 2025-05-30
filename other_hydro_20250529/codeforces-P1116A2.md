## Description

<div><p>You are given $N$ qubits in the zero state $|0...0 \rangle$. You are also given four distinct bit vectors which describe four different basis states on $N$ qubits $|\psi_i \rangle$.</p><p>Your task is to generate a state which is an equal superposition of the given basis states:</p><p>$$|S \rangle = \frac{1}{2} \big( |\psi_0 \rangle + |\psi_1 \rangle + |\psi_2 \rangle + |\psi_3 \rangle \big)$$</p><p>You have to implement an operation which takes the following inputs:</p><ul><li> an array of $N$ ($2 \le N \le 16$) qubits,</li><li> a two-dimensional array of Boolean values $bits$ representing the basis states $|\psi_i \rangle$. $bits$ will have exactly 4 elements, each of $bits[i]$ describing the basis state $|\psi_i \rangle$. Each of $bits[i]$ will have $N$ elements, $bits[i][j]$ giving the state of qubit $j$ in the basis state $|\psi_i \rangle$. Bit values true and false corresponding to $|1 \rangle$ and $|0 \rangle$ states, respectively; for example, for $N = 2$ an array <span class="tex-font-style-tt">[false, true]</span> will represent the basis state $|01\rangle$. Each pair of $bits[i]$ and $bits[j]$ will differ in at least one position for $i \neq j$.</li></ul><p>The operation doesn't have an output; its "output" is the state in which it leaves the qubits.</p><p>Your code should have the following signature:</p><pre class="verbatim">namespace Solution {
    open Microsoft.Quantum.Primitive;
    open Microsoft.Quantum.Canon;

    operation Solve (qs : Qubit[], bits : Bool[][]) : Unit {
        // your code here
    }
}</pre></div>
