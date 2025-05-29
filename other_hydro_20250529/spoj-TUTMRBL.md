<p>Playing with marbles is one of the king's favorite pastimes. He especially enjoys a game which was taught to him by Eratosthenes, a visiting mathematician from Greece. The rules are very complicated but it all boils down to arranging marbles in a (filled) rectangular shape to score points. If playing with 24 marbles, for example, King Tut could make a 4 by 6 rectangle, or a 3 by 8 rectangle, or a 2 by 12 rectangle. Even the boring 1 by 24 rectangle is allowed. Other numbers of marbles, however, such as 23, make things difficult for the king. Try as he might, the only rectangle he can make is 1 by 23. (Note that rectangles are equivalent under rotation, so a 23 by 1 rectangle would not be a new shape.)</p>
<p>King Tut has decided to call numbers n which can form only the unexciting 1 by n rectangle "non-rectangular." Conversely, numbers like 24, which allow for the formation of more than one rectangle, shall henceforth be referred to as "rectangular." Playing with a single marble is not very interesting at all, so the number 1 will by definition considered neither rectangular nor non-rectangular.</p>
<p>After playing for some time, the king started to notice that every integer greater than 1 could be written as a product of non-rectangular numbers. Were he a mathematician, he would try to prove this claim (which, incidentally, is true). However, the king is more of the engineer type, so he's going to make you verify the claim using brute force! While you're at it, also tell the king how many rectangles can be constructed given a certain number of marbles.</p>
<h3>Input</h3>
<p>There will be several test cases, one per line, each consisting of a single integer between 2 and 10<sup>7</sup> inclusive. An input of zero will be used to tell your program to stop processing.</p>
<h3>Output</h3>
<p>For each test case, print out two lines! The first should show the given number of marbles written as a product of non-rectangular numbers, following the example of the sample output. Factors must be written in non-decreasing order and separated by multiplication signs. Also print out spaces around the equals and multiplication signs to improve readability. The second line of output for each test case should be in the format: "With X marbles, Y different rectangles can be constructed." Again, don't forget to replace X and Y with the proper values.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
24
23
0

<strong>Output:</strong>
24 = 2 * 2 * 2 * 3
With 24 marbles, 4 different rectangles can be constructed.
23 = 23
With 23 marbles, 1 different rectangles can be constructed.
</pre>