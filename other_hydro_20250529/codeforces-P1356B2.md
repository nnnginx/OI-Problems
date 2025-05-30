## Description

<div><p>Implement a unitary operation on a register of $N$ qubits that decrements the number written in the register modulo $2^N$.</p><p>Your operation should take a register of type <a href="https://docs.microsoft.com/en-us/qsharp/api/qsharp/microsoft.quantum.arithmetic.littleendian"><span class="tex-font-style-tt">LittleEndian</span></a> - an array of qubits that encodes an unsigned integer in little-endian format, with the least significant bit written first (corresponding to the array element with index 0). The "output" of your solution is the state in which it left the input qubits.</p><p>For example, if the qubits passed to your operation are in the state $\frac{1}{\sqrt{2}}(|00\rangle + |01\rangle) = \frac{1}{\sqrt{2}}(|0\rangle + |2\rangle)$, they should be transformed to the state $\frac{1}{\sqrt{2}}(|(0-1) \mod 2^2\rangle + |(2-1) \mod 2^2\rangle) = \frac{1}{\sqrt{2}}(|3\rangle + |1\rangle) = \frac{1}{\sqrt{2}}(|11\rangle + |10\rangle)$.</p><p>Your code should have the following signature (note that your operation should have Adjoint and Controlled variants defined for it; <span class="tex-font-style-tt">is Adj+Ctl</span> in the operation signature will generate them automatically based on your code):</p><pre class="verbatim">namespace Solution {
    open Microsoft.Quantum.Arithmetic;
    open Microsoft.Quantum.Intrinsic;

    operation Solve (register : LittleEndian) : Unit is Adj+Ctl {
        // your code here
    }
}</pre><p>Your code is not allowed to use measurements or arbitrary rotation gates (so, for example, using the library operation <a href="https://docs.microsoft.com/en-us/qsharp/api/qsharp/microsoft.quantum.arithmetic.incrementbyinteger">IncrementByInteger</a> will cause runtime error). This operation can be implemented using just the X gate and its controlled variants.</p></div>
