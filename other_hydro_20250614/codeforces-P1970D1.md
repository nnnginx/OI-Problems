## Description

<div><p>Professor Vector is preparing to teach her Arithmancy class. She needs to prepare $n$ distinct <span class="tex-font-style-it">magic words</span> for the class. Each magic word is a string consisting of characters <span class="tex-font-style-tt">X</span> and <span class="tex-font-style-tt">O</span>. A <span class="tex-font-style-it">spell</span> is a string created by concatenating two magic words together. The <span class="tex-font-style-it">power</span> of a spell is equal to the number of its different non-empty substrings. For example, the power of the spell <span class="tex-font-style-tt">XOXO</span> is equal to 7, because it has 7 different substrings: <span class="tex-font-style-tt">X</span>, <span class="tex-font-style-tt">O</span>, <span class="tex-font-style-tt">XO</span>, <span class="tex-font-style-tt">OX</span>, <span class="tex-font-style-tt">XOX</span>, <span class="tex-font-style-tt">OXO</span> and <span class="tex-font-style-tt">XOXO</span>.</p><p>Each student will create their own spell by concatenating two magic words. Since the students are not very good at magic yet, they will choose each of the two words independently and uniformly at random from the $n$ words provided by Professor Vector. It is therefore also possible that the two words a student chooses are the same. Each student will then compute the power of their spell, and tell it to Professor Vector. In order to check their work, and of course to impress the students, Professor Vector needs to find out which two magic words and in which order were concatenated by each student.</p><p>Your program needs to perform the role of Professor Vector: first, create $n$ distinct magic words, and then handle multiple requests where it is given the spell power and needs to determine the indices of the two magic words, in the correct order, that were used to create the corresponding spell.</p></div><div><h2>Interaction</h2><p><span class="tex-font-style-it">This is an interactive problem.</span></p><p>First, your program should read a single integer $n$ ($1 \le n \le 3$), the number of magic words to prepare. Then, it should print $n$ magic words it has created, one per line. The magic words must be distinct, each magic word must have at least 1 and at most $30\cdot n$ characters, and each character must be either <span class="tex-font-style-tt">X</span> or <span class="tex-font-style-tt">O</span>. We will denote the $i$-th magic word you printed as $w_i$ ($1 \le i \le n$).</p><p>Then, your program should read a single integer $q$ ($1 \le q \le 1000$), the number of students in the class. Then, it should repeat the following process $q$ times, one per student.</p><p>For the $j$-th student, it should first read a single integer $p_j$, the power of their spell. It is guaranteed that this number is computed by choosing two indices $u_j$ and $v_j$ independently and uniformly at random between 1 and $n$ inclusive, concatenating $w_{u_j}$ and $w_{v_j}$, and finding the number of different non-empty substrings of the resulting string. Then, your program must print the numbers $u_j$ and $v_j$, in this order ($1 \le u_j, v_j \le n$).</p><p>Note that it is not enough to find any two magic words that concatenate into a spell with the given power. You must find the exact words used by the student in the exact order.</p><p>Remember to flush the output stream after printing all magic words and after printing $u_j$ and $v_j$ for each student.</p></div>





```input1
2


2
15

11
```




```output1
XOXO
X


1 1

2 1
```


