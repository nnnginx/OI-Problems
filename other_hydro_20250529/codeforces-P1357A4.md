## Description

<div><p>You are given an operation that implements a single-qubit unitary transformation: either the Rz gate or the R1 gate. The operation will have Adjoint and Controlled variants defined.</p><p>Your task is to perform necessary operations and measurements to figure out which unitary it was and to return 0 if it was the Rz gate or 1 if it was the R1 gate. </p><p>You are allowed to apply the given operation and its adjoint/controlled variants exactly once (you can pass to it any rotation angle that you choose).</p><p>You have to implement an operation which takes a single-qubit operation <span class="tex-font-style-tt">unitary</span> as an input and returns an integer. The operation <span class="tex-font-style-tt">unitary</span> will accept two parameters (similarly to <a href="https://docs.microsoft.com/en-us/qsharp/api/qsharp/microsoft.quantum.intrinsic.rz">Rz</a> and <a href="https://docs.microsoft.com/en-us/qsharp/api/qsharp/microsoft.quantum.intrinsic.r1">R1</a> intrinsic gates): the first parameter is the rotation angle and the second parameter is the qubit to which the rotation is applied. Your code should have the following signature:</p><pre class="verbatim">namespace Solution {
    open Microsoft.Quantum.Intrinsic;

    operation Solve (unitary : ((Double, Qubit) =&gt; Unit is Adj+Ctl)) : Int {
        // your code here
    }
}</pre></div>
