## Description

<div><p>You are given a qubit which is guaranteed to be either in <img align="middle" class="tex-formula" src="./29384/file/yOseyM7r.png" style="max-width: 100.0%;max-height: 100.0%;"> state or in <img align="middle" class="tex-formula" src="./29384/file/NKUPfbF0.png" style="max-width: 100.0%;max-height: 100.0%;"> state. </p><p>Your task is to perform necessary operations and measurements to figure out which state it was and to return 0 if it was a <img align="middle" class="tex-formula" src="./29384/file/FH0Uy9Kj.png" style="max-width: 100.0%;max-height: 100.0%;"> state, 1 if it was <img align="middle" class="tex-formula" src="./29384/file/YEbg9Hbb.png" style="max-width: 100.0%;max-height: 100.0%;"> state or -1 if you can not decide, i.e., an "inconclusive" result. The state of the qubit after the operations does not matter.</p><p>Note that these states are not orthogonal, and thus can not be distinguished perfectly. In each test your solution will be called 10000 times, and your goals are:</p><ul><li> never give 0 or 1 answer incorrectly (i.e., never return 0 if input state was <img align="middle" class="tex-formula" src="./29384/file/5y2OUFjg.png" style="max-width: 100.0%;max-height: 100.0%;"> and never return 1 if input state was <img align="middle" class="tex-formula" src="./29384/file/HMzHneKX.png" style="max-width: 100.0%;max-height: 100.0%;">),</li><li> give -1 answer at most 80% of the times,</li><li> correctly identify <img align="middle" class="tex-formula" src="./29384/file/wgD5q2JL.png" style="max-width: 100.0%;max-height: 100.0%;"> state at least 10% of the times,</li><li> correctly identify <img align="middle" class="tex-formula" src="./29384/file/YpuT6VHL.png" style="max-width: 100.0%;max-height: 100.0%;"> state at least 10% of the times.</li></ul><p>In each test <img align="middle" class="tex-formula" src="./29384/file/XHQXC2yj.png" style="max-width: 100.0%;max-height: 100.0%;"> and <img align="middle" class="tex-formula" src="./29384/file/xqQfMZti.png" style="max-width: 100.0%;max-height: 100.0%;"> states will be provided with 50% probability.</p><p>You have to implement an operation which takes a qubit as an input and returns an integer. </p><p>Your code should have the following signature:</p><pre class="verbatim">namespace Solution {
    open Microsoft.Quantum.Primitive;
    open Microsoft.Quantum.Canon;

    operation Solve (q : Qubit) : Int
    {
        body
        {
            // your code here
        }
    }
}</pre></div>
