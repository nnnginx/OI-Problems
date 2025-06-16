## Description

<div><p>You are given a qubit which is guaranteed to be either in <img align="middle" class="tex-formula" src="./29383/file/8X1t61uC.png" style="max-width: 100.0%;max-height: 100.0%;"> state or in <img align="middle" class="tex-formula" src="./29383/file/5FdRkXkt.png" style="max-width: 100.0%;max-height: 100.0%;"> state. </p><p>Your task is to perform necessary operations and measurements to figure out which state it was and to return 0 if it was a <img align="middle" class="tex-formula" src="./29383/file/IKx06csW.png" style="max-width: 100.0%;max-height: 100.0%;"> state or 1 if it was <img align="middle" class="tex-formula" src="./29383/file/GE9SJWjf.png" style="max-width: 100.0%;max-height: 100.0%;"> state. The state of the qubit after the operations does not matter.</p><p>Note that these states are not orthogonal, and thus can not be distinguished perfectly. In each test your solution will be called 1000 times, and your goal is to get a correct answer at least 80% of the times. In each test <img align="middle" class="tex-formula" src="./29383/file/LdqZXxB2.png" style="max-width: 100.0%;max-height: 100.0%;"> and <img align="middle" class="tex-formula" src="./29383/file/2hQVepHM.png" style="max-width: 100.0%;max-height: 100.0%;"> states will be provided with 50% probability.</p><p>You have to implement an operation which takes a qubit as an input and returns an integer. </p><p>Your code should have the following signature:</p><pre class="verbatim">namespace Solution {
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
