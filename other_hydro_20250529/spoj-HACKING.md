<p>A coach of one of the soccer world finals teams (lets call him Hugo Hacker) wants to find out secret information about an opposing team before the game. The coach of the opposing team has a website with public information about his team. Hugo suspects that also secret information is stored on the computer which hosts the website.</p>
<p>The website contains a form which allows to search for key words and returns a chunk of a text file which contains the key word. Hugo has found out that by entering words which cannot be found in the documents publicly available, he can exploit a bug in the search and get access to other files on the computer. He already knows the publicly available documents. However the search box has a restriction on the maximum length of a word and the characters which can be entered. Can you tell him a word which can be entered in the search box and which does not occur as a substring in the documents?</p>
<h3>Input</h3>
<p>The first line of the input consists of the number of test cases which are to follow. Each test case consists of two lines: in the first line there are three integers <em>n</em> (<em>1 ¡Ü n ¡Ü 10000</em>), <em>m</em> (<em>1 ¡Ü m ¡Ü 100</em>) and <em>k</em> (<em>1 ¡Ü k ¡Ü 26</em>), where <em>n</em> is the length of the publicly available documents, <em>m</em> is the maximum allowed length of words which can be entered in the search box, and <em>k</em> specifies that the search box allows only the first <em>k</em> characters of the alphabet. The second line of each test case describes the publicly available documents and consists of <em>n</em> lower-case letters.</p>
<h3>Output</h3>
<p>For each test case in the input, print one line in the output containing a word which does not occur as a substring in the given text. The word should have at most <em>m</em> lower-case characters from the first <em>k</em> letters in the alphabet. You may assume that for each given test case, there is always at least one such word (you may print any such word).</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
9 3 2
bbbaababb
9 3 2
aaabbabaa

<strong>Output:</strong>
aaa
bbb
</pre>