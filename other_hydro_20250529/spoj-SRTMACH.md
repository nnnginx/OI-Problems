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
<p>
Once upon a time, there was a machine, a sorting machine called Conchita, she was not very efficient,  most of the times she even couldn't sort the data correctly, and she only could process a list of $2 \le N \le 10$ numbers,  her algorithm was the following, she was programmed with 2 permutations of $N$ numbers, each permutation $F$ is given by $N$ numbers, 
$f_1, f_2, \ldots, f_N$, such that $1 \le f_i \le N$, $f_i \ne f_j$ for $i \ne j$ and means that if she apply $F$ to the given list, she gets a list where the $f_i$ element, corresponds to the $i$ element on the original list, then she forms a set of rearrangements of the original list, applying any of these permutations any number of times, in any order to the given list, so she forms all possible rearrangements using the given permutations, then she chooses to output the one that minimize the first element, if there is any tie, she chooses the one that minimize the second element and if there is any tie, she looks at the third element, and so on... </p>

<p>
Her creator, a robot called Robotina, was very curious about Conchita's behavior, she chooses an integer $1 \le M \le 10$, an then she tries all possible lists, $a_1, a_2, \ldots, a_N$, such that $1 \le a_i \le M$, and then for each input, she sends it to Conchita, and receives an output, then she asks herself, how many possible different outputs does Conchita can compute? (Two outputs are considered different if at least one element differs).</p>

<p>Your task, find this number MOD $98765431$.</p>

<h3>Input</h3>
<p>
The first line of input contains an integer $T \le 10$, the number of test cases. 
It is followed by $T$ test cases, the first line of each test case contains 2 integer numbers, $N$, $M$, then is followed by 2 lines, each one consisting on $N$ numbers.
</p>

<h3>Output</h3>
<p>For each case, output a single line consisting of the number of different outputs MOD $98765431$.</p>

<h4>Input Sample</h4>
<pre>2
2 2
1 2
2 1
3 3
2 1 3
3 1 2
</pre>

<h4>Output sample</h4>
<pre>3
10
</pre>