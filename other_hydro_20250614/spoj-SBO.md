<p>Given a sequence of numbers, each number between 1 and 100000 (inclusive), find the contiguous subsequence with maximum rarity.</p>
<p>The rarity of a sequence is defined as the count of numbers which appear only once in that sequence. For example, let's consider the following sequence:</p>
<p>1 1 2 5 1 16 5</p>
<p>The rarity of the subsequence 1 1 2 5 is 2. This is because 2 and 5 are the only numbers which appear just once. 1 appears twice in the sequence, hence doesn't contribute to it's rarity. The rarity of subsequence 1 16 5 is 3 as each of the numbers appears only once. The maximum rarity achieved by any contiguous subsequence in the sequence 1 1 2 5 1 16 5 is 4. This is the rarity of 2 5 1 16.</p>
<p>Your task is to find the contiguous subsequence with maximum rarity and output that rarity value. You don't have to output the subsequence itself.</p>
<h3>Input</h3>
<p>The first line of input will contain an integer N. N is the count of numbers in the input sequence.</p>
<p>1&lt;=N&lt;=500000.</p>
<p>The next line will contain the sequence of numbers. Each number in the sequence is an integer between 1 and 100000.</p>
<h3>Output</h3>
<p>The maximum rarity that any contiguous subsequence possesses.</p>
<h3>Example</h3>
<pre><strong>Input 1:</strong>
7<br>1 1 2 5 1 16 5<br><strong>Output 1:</strong>
4<br><br><strong>Input 2:<br></strong>3<br>1 2 3<br><strong>Output 2:<br></strong>3<br><strong><br>Input 3:<br></strong>10<br>2 1 4 1 5 6 7 1 8 2<br><strong>Output 3:<br></strong>6<br><strong><br>Input 4:<br></strong>20<br>3 4 14 14 9 7 11 7 15 13 9 9 14 9 13 10 13 9 5 4<strong><br>Output 4:<br></strong>7<br><br><strong>Explanation:<br>Input 2: </strong>The maximum rarity is achieved by the sequence itself.<br><strong>Input 3: </strong>The maximum rarity is achieved by the subsequences 1 4 1 5 6 7 1 8 2, 4 1 5 6 7 1 8 2 and 5 6 7 1 8 2.<br>            All the three contiguous subsequences have rarity 6.<strong><br>Input 4: </strong>The maximum rarity is achieved by the subsequence 11 7 15 13 9 9 14 9 13 10 13 9 5 4.<br>            This sequence has 7 numbers which appear only once in it, i.e., 11, 7, 15, 14, 10, 5, 4.</pre>