<p>Natalia has another problem she needs your help with. Do you still have some energies left?</p>
<p>A <em>Logical String</em>&nbsp;is a string that represents a valid boolean expression. It is composed of operators AND, OR and NOT and truth values operands. The boolean expressions are recursive in the sense that operators can have other operators as operands. For example, the following is a list of valid <em>Logical Strings</em>:</p>
<p><span style="white-space: pre;">T<br></span>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; T<br><span style="white-space: pre;">F<br></span>&nbsp; F<br><span style="white-space: pre;">AND(T, T)<br></span><span style="white-space: pre;">OR(T, F)<br></span><span style="white-space: pre;">NOT(T)<br></span><span style="white-space: pre;">AND(OR(T, F), AND(F, F))<br></span><span style="white-space: pre;">AND(AND(AND(OR(T, F), F), F), T)<br></span><span style="white-space: pre;">AND    (    AND     ( OR        ( T,F),OR(F,F)),T)</span></p>
<p><span style="white-space: pre;">&nbsp;</span></p>
<p>Please note that there can be several spaces in between objects. However, no space will be in between letters of the names. Therefore, "AND(T,T)" is a valid <em>Logical String</em>&nbsp;but "A &nbsp; &nbsp; N &nbsp; &nbsp; &nbsp; D(T,T)" is not.</p>
<p><span style="white-space: pre;">Given a <em>Logical String</em>, please evaluate it and output its truth value.</span></p>
<h3>Input</h3>
<p>The first line contains T(1¡Ü T ¡Ü 100), the number of test cases. Then there are T lines. Each line contains a string s<sub>0</sub>s<sub>1</sub>s<sub>2</sub>...s<sub>n-1</sub>(1 ¡Ü N ¡Ü 100). It is guaranteed that the i<sup>th</sup> <em>Logical String</em>&nbsp;is valid.</p>
<h3>Output</h3>
<p>For each <em>Logical String</em>&nbsp;given, output its truth value. If it is true, output T, otherwise output F.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<p>7<br>T<br>F<br>AND(T, T)<br>OR(T, F)<br>NOT(T)<br>AND(OR(T, F), AND(F, F))<br>AND(AND(AND(OR(T, F), F), F), T)</p></pre>
<pre><strong>Output:</strong>
<p>T<br>F<br>T<br>T<br>F<br>F<br>F</p></pre>