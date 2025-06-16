## Description

<div><p>You are given <span class="tex-span"><i>N</i></span> qubits which are guaranteed to be in one of two basis states on <span class="tex-span"><i>N</i></span> qubits. You are also given two bitstrings <span class="tex-span"><i>bits</i>0</span> and <span class="tex-span"><i>bits</i>1</span> which describe these basis states.</p><p>Your task is to perform necessary operations and measurements to figure out which state it was and to return 0 if it was the state described with <span class="tex-span"><i>bits</i>0</span> or 1 if it was the state described with <span class="tex-span"><i>bits</i>1</span>. The state of the qubits after the operations does not matter.</p></div><div class="input-specification"><p>You have to implement an operation which takes the following inputs:</p><ul><li> an array of qubits <span class="tex-span"><i>qs</i></span>,</li><li> two arrays of boolean values <span class="tex-span"><i>bits</i>0</span> and <span class="tex-span"><i>bits</i>1</span>, representing the basis states in which the qubits can be. These arrays will have the same length as the array of qubits. <span class="tex-span"><i>bits</i>0</span> and <span class="tex-span"><i>bits</i>1</span> will differ in at least one position.</li></ul><p>An array of boolean values represents a basis state as follows: the <span class="tex-span"><i>i</i></span>-th element of the array is true if the <span class="tex-span"><i>i</i></span>-th qubit is in state <img align="middle" class="tex-formula" src="./29370/file/gm7RRxNC.png" style="max-width: 100.0%;max-height: 100.0%;">, and false if it is in state <img align="middle" class="tex-formula" src="./29370/file/jTbIXEEk.png" style="max-width: 100.0%;max-height: 100.0%;">. For example, array [true; false] describes 2-qubit state <img align="middle" class="tex-formula" src="./29370/file/IPgruBs2.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>Your code should have the following signature:</p><pre class="verbatim">namespace Solution {
    open Microsoft.Quantum.Primitive;
    open Microsoft.Quantum.Canon;

    operation Solve (qs : Qubit[], bits0 : Bool[], bits1 : Bool[]) : Int
    {
        body
        {
            // your code here
        }
    }
}</pre></div>

## Input

<p>You have to implement an operation which takes the following inputs:</p><ul><li> an array of qubits <span class="tex-span"><i>qs</i></span>,</li><li> two arrays of boolean values <span class="tex-span"><i>bits</i>0</span> and <span class="tex-span"><i>bits</i>1</span>, representing the basis states in which the qubits can be. These arrays will have the same length as the array of qubits. <span class="tex-span"><i>bits</i>0</span> and <span class="tex-span"><i>bits</i>1</span> will differ in at least one position.</li></ul><p>An array of boolean values represents a basis state as follows: the <span class="tex-span"><i>i</i></span>-th element of the array is true if the <span class="tex-span"><i>i</i></span>-th qubit is in state <img align="middle" class="tex-formula" src="./29370/file/gm7RRxNC.png" style="max-width: 100.0%;max-height: 100.0%;">, and false if it is in state <img align="middle" class="tex-formula" src="./29370/file/jTbIXEEk.png" style="max-width: 100.0%;max-height: 100.0%;">. For example, array [true; false] describes 2-qubit state <img align="middle" class="tex-formula" src="./29370/file/IPgruBs2.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>Your code should have the following signature:</p><pre class="verbatim">namespace Solution {
    open Microsoft.Quantum.Primitive;
    open Microsoft.Quantum.Canon;

    operation Solve (qs : Qubit[], bits0 : Bool[], bits1 : Bool[]) : Int
    {
        body
        {
            // your code here
        }
    }
}</pre>
