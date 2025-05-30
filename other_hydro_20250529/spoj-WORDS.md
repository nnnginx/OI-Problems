<p>
Consider the following game: you are given a word W that contains only lower-case letters ("a" to "z"). You are also given a set of words and you are allowed to do the following operation: choose a suffix of W and replace it with another word (you can do this only if that word contains the suffix as its prefix). For example, if the current words is "acmicpc" you can choose to replace the suffix "pc" with any word in the set you are given that starts with "pc", e.g. "pcaaargh" thus forming the word "acmicpcaaargh". You can then repeat this procedure as many times as you wish. You are free to choose any suffix of the current word as long as it matches a prefix of the word you are replacing it with. You can also choose not to do the operation at all. Each suffix you replace must have length at least 1 (you cannot replace the "null suffix" with a word). 

</p><p>You are also given an integer L, 1 �� L �� 5. Your task is to find how many different subwords of length exactly L can be produced using the following operation. A "subword" means a substring of length L.

</p><h3>Input</h3>
<p>The first line of the input file contains two integers, N and L separated by space. N, 1 �� N �� 100 is the number of words in the set (including the initial word). The next N lines describe one word each. No other symbols except small latin letters, and the end-of-line symbol are found on these lines.
Each word has length at least L and at most 128. The word you start with is the first word in this set.

</p><h3>Output</h3>
<p>The only line of the output should contain one integer: the number of different subwords of length L that can be produced using the operation described above.

</p><h3>Example</h3>

<pre><b>Input:</b>
2 5
acmicpc
pcaaaaaaargh

<b>Output:</b>
11
</pre>