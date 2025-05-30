## Description

<div><p>You are given an operation that implements a single-qubit unitary transformation: either the Y gate (possibly with an extra global phase of $-1$) or the sequence of Pauli Z and Pauli X gates (the Z gate applied first and the X gate applied second; possibly with an extra global phase of $-1$). The operation will have Adjoint and Controlled variants defined.</p><p>Your task is to perform necessary operations and measurements to figure out which unitary it was and to return</p><ul> <li> 0 if it was the Y gate, </li><li> 1 if it was the $-$XZ gate, </li><li> 2 if it was the $-$Y gate, </li><li> 3 if it was the XZ gate. </li></ul><p>You are allowed to apply the given operation and its adjoint/controlled variants <span class="tex-font-style-bf">at most three times</span>.</p><p>You have to implement an operation which takes a single-qubit operation as an input and returns an integer. Your code should have the following signature:</p><pre class="verbatim">namespace Solution {
    open Microsoft.Quantum.Intrinsic;

    operation Solve (unitary : (Qubit =&gt; Unit is Adj+Ctl)) : Int {
        // your code here
    }
}</pre></div>
