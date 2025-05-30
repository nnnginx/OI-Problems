## Description

<div><p>You are given an operation that implements a single-qubit unitary transformation: either the H gate or the X gate. The operation will have Adjoint and Controlled variants defined.</p><p>Your task is to perform necessary operations and measurements to figure out which unitary it was and to return 0 if it was the H gate or 1 if it was the X gate. </p><p>You are allowed to apply the given operation and its adjoint/controlled variants <span class="tex-font-style-bf">at most twice</span>.</p><p>You have to implement an operation which takes a single-qubit operation as an input and returns an integer. Your code should have the following signature:</p><pre class="verbatim">namespace Solution {
    open Microsoft.Quantum.Intrinsic;

    operation Solve (unitary : (Qubit =&gt; Unit is Adj+Ctl)) : Int {
        // your code here
    }
}</pre></div>
