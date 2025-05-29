<p>You are given a permutation of first N natural numbers on which you are to perform K operations of following type: given integers A and B, your task is to swap elements on positions A and B in permutation and then output permutation rank modulo 1000 000 007.</p>
<p><strong>Note:</strong> Difference from original task is that elements remain swapped after query.</p>
<h3>Input</h3>
<p>On first line of standard input you are given two integers (2 ¡Ü N ¡Ü 50 000, 1 ¡Ü K ¡Ü 30 000), length of permutation and number of operations.<br>On the next line there is permutation of first N natural numbers.<br>In next K lines there are two integers A, B ( 1 ¡Ü A, B ¡Ü N ).</p>
<h3>Output</h3>
<p>Output permutation rank after applying each of K operations.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>5 3<br>1 5 4 2 3<br>1 3<br>2 3<br>2 5<br><br><strong>Output:</strong><br>91<br>77<br>90<br></pre>