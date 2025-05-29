<p>The most common technique for shuffling a deck of cards is called the Riffle or Dovetail shuffle. The deck is split into two stacks, which are then interleaved with each other. The deck can be split anywhere, and the two stacks can be interleaved in any way.</p>
<p>For example, consider a deck with 10 unique cards:</p>
<p style="text-align: left;"><strong>1 2 3 4 5 6 7 8 9 10</strong></p>
<p>Split them somewhere:</p>
<p>1 2 3 4 5 6 &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;7 8 9 10</p>
<p>And interleave them in some way:</p>
<p>1 2 7 3 8 9 4 5 10 6</p>
<p>Do it again. Split them somewhere:</p>
<p>1 2 7 &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;3&nbsp;8 9 4 5 10 6</p>
<p>And interleave them in some way:</p>
<p>3 8 1 9 4 5 2 7 10 6</p>
<p>This is one possible ordering after 2 shuffles. Suppose there are <strong>n</strong> unique cards, and that they start out perfectly ordered: 1, 2, 3, ..., <strong>n</strong>. Given an ordering of the deck, what is the smallest number of shuffles that could possibly put the deck in that order?</p>
<h3>Input</h3>
<p>Each input will consist of a single test case. Note that your program may be run multiple times on different inputs. Each test case will begin with a single integer <strong>n</strong> (1¡Ü<strong>n</strong>¡Ü1,000,000) indicating the number of cards in the deck. On the next line will be <strong>n</strong> unique integers <strong>c</strong> (1¡Ü<strong>c</strong>¡Ü<strong>n</strong>), with a single space between them, indicating an ordering of the <strong>n</strong> cards. The values <strong>c</strong> are guaranteed to be a permutation of the numbers 1..<strong>n</strong>.</p>
<h3>Output</h3>
<p>Output a single line with a single integer indicating the minimum number of shuffles that could possibly put the deck in the given order. Output no spaces.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
10 <br>1 2 7 3 8 9 4 5 10 6

<strong>Output:</strong>
1</pre>
<pre><strong>Input:</strong>
8 <br>2 1 4 3 6 5 8 7

<strong>Output:</strong>
3</pre>
<pre><strong>Input:</strong>
10 <br>3 8 1 9 4 5 2 7 10 6

<strong>Output:</strong>
2</pre>