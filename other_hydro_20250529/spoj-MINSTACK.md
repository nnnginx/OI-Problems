<div>
<p>Every Christmas the good old man can go to every  house in the world and leave gifts for the children who have been good  throughout the year, but this is only possible because of his magic gift  bag. It would be impossible for Santa to carry all the presents in his  bag, the volume and weight of them all makes this obviously unfeasible.  What actually happens is that your bag is a kind of magical portal to  your gift factory at the North Pole. Where the presents are stacked by  their elves and Noel always takes the gift from the top of that pile  when he accesses his magical bag.</p>
<p>Gifts have a numerical measure of the degree of fun  they can provide children, and Santa is always concerned with the least  fun gift he will deliver throughout the night because he does not want  any child to feel bad about it. you receive. However, this can not be  done in advance because throughout the night as the good old man takes  gifts from the pile to deliver, others are still being made and placed  on the pile. So the most he can know is the value of the least fun  present on the stack up to that point.</p>
<p>Your task is, given the sequence of operations done  on the stack of gifts, answer Santa's queries about the value of the  least entertaining gift on the stack thus far.</p>
</div>
<h3>Input</h3>
<p>The first line of the input contains an integer <strong>N</strong> (1 ¡Ü <strong>N</strong> ¡Ü 10<sup>6</sup>) corresponding to the number of operations performed on the present stack. The operations can be of three types: "<em>PUSH</em> V" where <strong>V</strong> (1 ¡Ü <strong>V</strong> ¡Ü 10<sup>9</sup>) is an integer representing the degree of fun of the present being placed on the stack; "<em>POP</em>" which represents that Santa Claus is taking a gift from the cell to deliver and "<em>MIN</em>" representing a Noel query to know the smallest gift value in the stack.</p>
<h3>Output</h3>
<p>The output consists of a line containing an integer with the smallest  present value in the stack for queries of type "MIN" or "EMPTY" for  "MIN" and "POP" operations when the stack is empty.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
 11<br> PUSH 5<br> PUSH 7<br> PUSH 3<br> PUSH 8<br> PUSH 10<br> MIN<br> POP<br> POP<br> MIN<br> POP<br> MIN

<strong>Output:</strong>
<p>3
</p><p>3
</p><p>5
</p></pre>
<h3>Example</h3>
<pre><strong>Input:</strong>
 9<br> PUSH 100<br> PUSH 50<br> MIN<br> PUSH 45<br> MIN<br> POP<br> MIN<br> POP<br> MIN
<strong>Output:</strong>
<p>50
</p><p>45
</p><p>50
</p><p>100</p></pre>