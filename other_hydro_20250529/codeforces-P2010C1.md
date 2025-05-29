## Description

<div><p><span class="tex-font-style-bf">This is a simplified version of the problem. It differs from the difficult one only in its constraints.</span></p><p>At the Berland State University, the local network between servers does not always operate without errors. When transmitting two <span class="tex-font-style-bf">identical</span> messages consecutively, an error may occur, resulting in the two messages merging into one. In this merging, the end of the first message coincides with the beginning of the second. Of course, the merging can only occur at identical characters. The length of the merging must be a positive number less than the length of the message text.</p><p>For example, when transmitting two messages "<span class="tex-font-style-tt">abrakadabra</span>" consecutively, it is possible that it will be transmitted with the described type of error, resulting in a message like "<span class="tex-font-style-tt">abrakadabrabrakadabra</span>" or "<span class="tex-font-style-tt">abrakadabrakadabra</span>' (in the first case, the merging occurred at one character, and in the second case, at four).</p><p>Given the received message <span class="katex"><i>t</i></span>, determine if it is possible that this is the result of an error of the described type in the operation of the local network, and if so, determine a possible value of <span class="katex"><i>s</i></span>.</p><p>A situation where two messages completely overlap each other should not be considered an error. For example, if the received message is "<span class="tex-font-style-tt">abcd</span>", it should be considered that there is no error in it. Similarly, simply appending one message after another is not a sign of an error. For instance, if the received message is "<span class="tex-font-style-tt">abcabc</span>", it should also be considered that there is no error in it.</p></div><div class="input-specification"><p>The input consists of a single non-empty string <span class="katex"><i>t</i></span>, consisting of lowercase letters of the Latin alphabet. The length of the string <span class="katex"><i>t</i></span> does not exceed <span class="katex">100</span> characters.</p></div><div class="output-specification"><p>If the message <span class="katex"><i>t</i></span> cannot contain an error, output "<span class="tex-font-style-tt">NO</span>" (without quotes) in a single line of output.</p><p>Otherwise, in the first line, output "<span class="tex-font-style-tt">YES</span>" (without quotes), and in the next line, output the string <span class="katex"><i>s</i></span> ¡ª a possible message that could have led to the error. If there are multiple possible answers, any of them is acceptable.</p></div>

## Input

<p>The input consists of a single non-empty string <span class="katex"><i>t</i></span>, consisting of lowercase letters of the Latin alphabet. The length of the string <span class="katex"><i>t</i></span> does not exceed <span class="katex">100</span> characters.</p>

## Output

<p>If the message <span class="katex"><i>t</i></span> cannot contain an error, output "<span class="tex-font-style-tt">NO</span>" (without quotes) in a single line of output.</p><p>Otherwise, in the first line, output "<span class="tex-font-style-tt">YES</span>" (without quotes), and in the next line, output the string <span class="katex"><i>s</i></span> ¡ª a possible message that could have led to the error. If there are multiple possible answers, any of them is acceptable.</p>





```input1
abrakadabrabrakadabra

```




```input2
acacacaca

```




```input3
abcabc

```




```input4
abababab

```




```input5
tatbt

```




```output1
YES
abrakadabra

```




```output2
YES
acaca

```




```output3
NO

```




```output4
YES
ababab

```




```output5
NO

```



## Note

<p>In the second example, a suitable answer could also be the string "<span class="tex-font-style-tt">acacaca</span>".</p>
