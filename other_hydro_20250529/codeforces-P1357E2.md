## Description

<div><p>Implement an operation that is equivalent to the operation QFT$^{1/P}$, where QFT is the <a href="https://en.wikipedia.org/wiki/Quantum_Fourier_transform">quantum Fourier transform</a>. In other words, your operation, applied $P$ times, should have the same effect as applying QFT. You can implement the required transformation up to a global phase.</p><p>Your operation should take the following inputs:</p><ul> <li> an integer $P$ ($2 \le P \le 8$). </li><li> a register of type <a href="https://docs.microsoft.com/en-us/qsharp/api/qsharp/microsoft.quantum.arithmetic.littleendian"><span class="tex-font-style-tt">LittleEndian</span></a> - a wrapper type for an array of qubits that encodes an unsigned integer in little-endian format, with the least significant bit written first (corresponding to the array element with index 0). (If you need to, you can convert it to an array type using unwrap operator: <span class="tex-font-style-tt">let qubitArray = inputRegister!;</span>.) The register will contain at most 7 qubits. </li></ul><p>The "output" of your solution is the state in which it left the input qubits.</p><p>Your code should have the following signature (note that your operation should have Adjoint and Controlled variants defined for it; <span class="tex-font-style-tt">is Adj+Ctl</span> in the operation signature will generate them automatically based on your code):</p><pre class="verbatim">namespace Solution {
    open Microsoft.Quantum.Arithmetic;
    open Microsoft.Quantum.Intrinsic;

    operation Solve (p : Int, inputRegister : LittleEndian) : Unit is Adj+Ctl {
        // your code here
    }
}</pre><p>You can learn more about QFT in <a href="https://github.com/microsoft/QuantumKatas/tree/master/QFT">this kata</a>. You are allowed to take advantage of library operations, including <a href="https://docs.microsoft.com/en-us/qsharp/api/qsharp/microsoft.quantum.canon.qftle"><span class="tex-font-style-tt">QFTLE</span></a>.</p></div>
