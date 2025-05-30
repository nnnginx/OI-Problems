## Description

<div><p>You are given an operation that implements a single-qubit unitary transformation: either the Z gate or the -Z gate (i.e., the $-|0\rangle\langle0| + |1\rangle\langle1|$ gate: $(-Z)(\alpha|0\rangle + \beta|1\rangle) = -\alpha|0\rangle + \beta|1\rangle$). The operation will have Adjoint and Controlled variants defined.</p><p>Your task is to perform necessary operations and measurements to figure out which unitary it was and to return 0 if it was the Z gate or 1 if it was the -Z gate. </p><p>You are allowed to apply the given operation and its adjoint/controlled variants exactly <span class="tex-font-style-bf">once</span>.</p><p>You have to implement an operation which takes a single-qubit operation as an input and returns an integer. Your code should have the following signature:</p><pre class="verbatim">namespace Solution {
    open Microsoft.Quantum.Intrinsic;

    operation Solve (unitary : (Qubit =&gt; Unit is Adj+Ctl)) : Int {
        // your code here
    }
}</pre></div>
