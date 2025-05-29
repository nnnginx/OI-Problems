<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/KaTeX/0.7.1/katex.min.css" integrity="sha384-wITovz90syo1dJWVh32uuETPVEtGigN07tkttEqPv+uR2SE/mbQcG7ATL28aI9H0" crossorigin="anonymous">
<script src="https://cdnjs.cloudflare.com/ajax/libs/KaTeX/0.7.1/katex.min.js" integrity="sha384-/y1Nn9+QQAipbNQWU65krzJralCnuOasHncUFXGkdwntGeSvQicrYkiUBwsgUqc1" crossorigin="anonymous"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/KaTeX/0.7.1/contrib/auto-render.min.js"></script>
<script>// <![CDATA[
document.addEventListener("DOMContentLoaded", function(){
  renderMathInElement(
    document.body,{
      delimiters: [
        {left: "$$", right: "$$", display: true},
        {left: "$", right: "$", display: false}]})});
// ]]></script>

<p>Let $x$ is a binary number with $n$ digits ($a_na_{n-1}a_{n-2}...a_2a_1$). And we can encode it as $G(x) = x \oplus \lfloor \frac{x}{2} \rfloor$ or as $C(x) = (2^n - x) \bmod 2^n$, where "$\oplus$" is bitwise XOR operation and "$\lfloor x \rfloor$" indicates the largest integer which is not greater than $x$.</p>
<p>For some reasons, Chiaki encodes her password $P$ into $G(P)$ and $C(P)$. Then she writes $G(P)$ and $C(P)$ in a paper. However, something terrible happened. A bug ate some parts of the paper, so some digits are unreadable now. Chiaki is so worried that she want you to determine the values of these digits using the readable digits.</p>
<h3>Input</h3>
<p>There are multiple test cases. The first line of input contains an integer $T$, indicating the number of test cases. For each test case:</p>
<p>There are $2$ lines of same number of digits describe $G(P)$ and $C(P)$. In every line, it only contains '1', '0' and '?'. Unreadable digits are denoted with symbol '?'. Digits are given from the most significant digit to the least significant digit.</p>
<p>It is guaranteed that the sum of all $|G(P)|$ does not exceed $10^6$.</p>
<h3>Output</h3>
<p>For each test case, if it is impossible to restore $G(P)$ and $C(P)$, you should output "IMPOSSIBLE" (without the quotes).</p>
<p>If $G(P)$ is unique, you should output "UNIQUE" (without the quotes) in the first line. Then output restored $G(P)$ and $C(P)$ in the same format.</p>
<p>If there are two or more possible $G(P)$ that can be restored using the readable digits. You should output "AMBIGUOUS" (without the quotes) and the number of possible $G(P)$. The number may be very large, so the answer should modulo $10^9 + 7$.</p>
<h3>Example</h3>
<h4>Input:</h4>
<pre>3
1110
0101
11??
01??
111?
100?
</pre>
<h4>Output:</h4>
<pre>UNIQUE
1110
0101
AMBIGUOUS 3
IMPOSSIBLE
</pre>