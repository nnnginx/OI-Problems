## Description

<div><p>Implement a unitary operation on $N$ qubits which is represented by a square matrix of size $2^N$ defined as follows:</p><ul><li> top right and bottom left quarters are filled with zero elements, </li><li> the top left quarter is the same pattern of size $2^{N-1}$ (for $N = 1$, the top left quarter is a non-zero element),</li><li> the bottom right quarter is filled with non-zero elements.</li></ul><p>For example, for $N = 3$ the matrix of the operation should have the following shape:</p><pre class="verbatim">X.......
.X......
..XX....
..XX....
....XXXX
....XXXX
....XXXX
....XXXX</pre><p>Here <span class="tex-font-style-tt">X</span> denotes a "non-zero" element of the matrix (a complex number which has the square of the absolute value greater than or equal to $10^{-5}$), and <span class="tex-font-style-tt">.</span> denotes a "zero" element of the matrix (a complex number which has the square of the absolute value less than $10^{-5}$).</p><p>The row and column indices of the matrix follow little endian format: the least significant bit of the index is stored first in the qubit array. Thus, the first column of the matrix gives you the coefficients of the basis states you'll get if you apply the unitary to the $|00..0\rangle$ basis state, the second column - to the $|10..0\rangle$ basis state etc. You can use the <a href="https://github.com/Microsoft/QuantumKatas/tree/master/utilities/DumpUnitary">DumpUnitary tool</a> to get the coefficients of the matrix your unitary implements (up to relative phases between columns) and the corresponding pattern of <span class="tex-font-style-tt">X</span>s and <span class="tex-font-style-tt">.</span>s.</p><p>You have to implement an operation which takes an array of $N$ ($2 \le N \le 5$) qubits as an input and applies the unitary transformation with the matrix of the described shape to it. If there are multiple unitaries which satisfy the requirements, you can implement any of them. The "output" of your operation is the pattern of the matrix coefficients implemented by it; you can see the testing harness in the <a href="https://github.com/Microsoft/QuantumKatas/tree/master/UnitaryPatterns">UnitaryPatterns</a> kata.</p><p>Your code should have the following signature:</p><pre class="verbatim">namespace Solution {
    open Microsoft.Quantum.Primitive;
    open Microsoft.Quantum.Canon;

    operation Solve (qs : Qubit[]) : Unit {
        // your code here
    }
}</pre><p>You are not allowed to use measurements in your operation.</p></div>
