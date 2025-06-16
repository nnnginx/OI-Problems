<p>In 1930 the first FIFA World Cup was held in Uruguay, and Uruguay won  the Cup in a dramatic final against Argentina. All of this seems like ages past, and now myth and legend rank around that historic first world cup.  Some even claim that the original trophy cup that was awarded to Uruguay for their victory has mythical powers and would grant any side the strength to win the World Cup.</p>
<p>Now that original cup has been lost in time, and even though its mythical powers are probably just stories, it is still an important artifact which belongs in a museum. Clearly an expert is needed to recover it.</p>
<p>Famous archaeologist and adventurer Indiana Jones has taken this dangerous  task onto himself and traveled to Uruguay to find the cup. His search has led him to an ancient underground cave system where the cup is rumoured to have been hidden. Many traps lure within these caves, and only his instinct and his faithful whip have saved Indy from certain death. Now he has reached a mysterious enormous gate and he can only speculate that the cup must be hidden behind that gate. Unfortunately it is shut close.</p>
<p>The gate is riddled with switches and levers, and all of them are denoted with letters and numbers. As you may have guessed, the gate will only open if the switches and levers are pulled in the correct order, but beware! - For if anyone is unlucky enough to get the order wrong, doom awaits him.</p>
<p>Luckily, during his exploration of the caves Indy has found several encrypted hints which provide clues about the correct sequence. Here's one: "The faithful knows that <em>X</em> comes before <em>O</em>" And another: "Under no circumstances should you touch <em>a</em> unless <em>b</em> has been moved!" Clearly these clues give hints about the correct order, but there are a lot of switches and levers, and there are lots of clues. Indy needs help!</p>
<p>Given all of the hints Indy has collected, can you help him determine the correct order of the levers and switches so that he can successfully  complete his adventure? But beware - Indy could have missed some hints; or perhaps he misinterpreted some of them. The former case will likely leave more than one possible sequence while the latter will lead to no possible sequence at all. You must detect these cases and warn Indy.</p>
<h3>Input</h3>
<p>The first line of input contains the number of test cases <em>C</em> (<em>C �� 30</em>). For each test case there is one line with the number <em>n</em> (<em>1 �� n �� 10<sup>4</sup></em>) of switches/levers on the gate and the number <em>h</em> (<em>0 �� h �� 10<sup>5</sup></em>) of hints that Indy has discovered. Then follow <em>h</em> lines, one for each clue, with the numbers <em>a</em> and <em>b</em> (<em>1 �� a,b �� n, a �� b</em>), meaning that lever <em>a</em> must be pulled before lever <em>b</em>.</p>
<h3>Output</h3>
<p>For each test case output one line with the correct sequence of the numbers  <em>1</em> to <em>n</em>. Separate the numbers with a whitespace. If there is no possible sequence, print <strong>recheck hints</strong> instead. Otherwise if there are multiple possible sequences, print <strong>missing hints</strong> instead.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3
3 2
1 2
3 1
3 1
1 2
3 2
1 2
2 1

<strong>Output:</strong>
3 1 2
missing hints
recheck hints
</pre>