## Description

<div><p>You are given an angle $\theta$ (in radians, $0.01\pi \le \theta \le 0.99 \pi$) and an operation that implements a single-qubit unitary transformation: either the $Rz(\theta)$ gate or the $Ry(\theta)$ gate. The operation will have Adjoint and Controlled variants defined.</p><p>Your task is to perform necessary operations and measurements to figure out which unitary it was and to return 0 if it was the $Rz(\theta)$ gate or 1 if it was the $Ry(\theta)$ gate. </p><p>You are allowed to apply the given operation and its adjoint/controlled variants as many times as you need (within the time limit).</p><p>You have to implement an operation which takes a floating-point number and a single-qubit operation as an input and returns an integer. Your code should have the following signature:</p><pre class="verbatim">namespace Solution {
    open Microsoft.Quantum.Intrinsic;

    operation Solve (theta : Double, unitary : (Qubit =&gt; Unit is Adj+Ctl)) : Int {
        // your code here
    }
}</pre></div>
