## Description

<div><p>You are given <span class="tex-span"><i>N</i></span> qubits (<span class="tex-span">1 ≤ <i>N</i> ≤ 8</span>) in zero state <img align="middle" class="tex-formula" src="./29376/file/Lub6e6XB.png" style="max-width: 100.0%;max-height: 100.0%;">. You are also given a bitstring <span class="tex-span"><i>bits</i></span> which describes a non-zero basis state on <span class="tex-span"><i>N</i></span> qubits <img align="middle" class="tex-formula" src="./29376/file/IfI2xx5I.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>Your task is to generate a state which is an equal superposition of <img align="middle" class="tex-formula" src="./29376/file/RNaCN2fC.png" style="max-width: 100.0%;max-height: 100.0%;"> and the given basis state:</p><center class="tex-equation"><img align="middle" class="tex-formula" src="./29376/file/1X8ykdJm.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>You have to implement an operation which takes the following inputs:</p><ul><li> an array of qubits <span class="tex-span"><i>qs</i></span>,</li><li> an arrays of boolean values <span class="tex-span"><i>bits</i></span> representing the basis state <img align="middle" class="tex-formula" src="./29376/file/BKQKEpSo.png" style="max-width: 100.0%;max-height: 100.0%;">. This array will have the same length as the array of qubits. The first element of this array <span class="tex-span"><i>bits</i>[0]</span> will be <span class="tex-font-style-tt">true</span>.</li></ul><p>The operation doesn't have an output; its "output" is the state in which it leaves the qubits.</p><p>An array of boolean values represents a basis state as follows: the <span class="tex-span"><i>i</i></span>-th element of the array is true if the <span class="tex-span"><i>i</i></span>-th qubit is in state <img align="middle" class="tex-formula" src="./29376/file/nnJhvlCl.png" style="max-width: 100.0%;max-height: 100.0%;">, and false if it is in state <img align="middle" class="tex-formula" src="./29376/file/A9B6RViW.png" style="max-width: 100.0%;max-height: 100.0%;">. For example, array <span class="tex-font-style-tt">[true; false]</span> describes 2-qubit state <img align="middle" class="tex-formula" src="./29376/file/Az31MBvN.png" style="max-width: 100.0%;max-height: 100.0%;">, and in this case the resulting state should be <img align="middle" class="tex-formula" src="./29376/file/tLIzo8Lo.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>Your code should have the following signature:</p><pre class="verbatim">namespace Solution {
    open Microsoft.Quantum.Primitive;
    open Microsoft.Quantum.Canon;

    operation Solve (qs : Qubit[], bits : Bool[]) : ()
    {
        body
        {
            // your code here
        }
    }
}</pre></div>
