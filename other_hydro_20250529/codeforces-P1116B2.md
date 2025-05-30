## Description

<div><p>You are given a qubit which is guaranteed to be in one of the following states:</p><ul><li> $|A\rangle = \frac{1}{\sqrt{2}} \big( |0\rangle + |1\rangle \big)$,</li><li> $|B\rangle = \frac{1}{\sqrt{2}} \big( |0\rangle + \omega |1\rangle \big)$, or</li><li> $|C\rangle = \frac{1}{\sqrt{2}} \big( |0\rangle + \omega^2 |1\rangle \big)$, where $\omega = e^{2i\pi/3}$.</li></ul><p>These states are not orthogonal, and thus can not be distinguished perfectly. Your task is to figure out in which state the qubit is <span class="tex-font-style-it">not</span>. More formally:</p><ul><li> If the qubit was in state $|A\rangle$, you have to return 1 or 2.</li><li> If the qubit was in state $|B\rangle$, you have to return 0 or 2.</li><li> If the qubit was in state $|C\rangle$, you have to return 0 or 1.</li><li> In other words, return 0 if you're sure the qubit was <span class="tex-font-style-it">not</span> in state $|A\rangle$, return 1 if you're sure the qubit was <span class="tex-font-style-it">not</span> in state $|B\rangle$, and return 2 if you're sure the qubit was <span class="tex-font-style-it">not</span> in state $|C\rangle$.</li></ul><p>Your solution will be called 1000 times, each time the state of the qubit will be chosen as $|A\rangle$, $|B\rangle$ or $|C\rangle$ with equal probability. The state of the qubit after the operations does not matter.</p><p>You have to implement an operation which takes a qubit as an input and returns an integer. Your code should have the following signature:</p><pre class="verbatim">namespace Solution {
    open Microsoft.Quantum.Primitive;
    open Microsoft.Quantum.Canon;

    operation Solve (q : Qubit) : Int {
        // your code here
    }
}</pre></div>
