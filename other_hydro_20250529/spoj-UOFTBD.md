<p>
<script type="text/x-mathjax-config">// <![CDATA[
MathJax.Hub.Config({tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}});
// ]]></script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
</p>
<p>Maybe you've played Diablo? There are three different character classes: Noobs, Suckers, and Pros. Noobs don't know anything about the game. Suckers think they know how to play. Pros know that the goal of the game is to write a script that will farm for valuable items that they can turn around and sell to Suckers on the black market. Obviously Pros would sell to Noobs if they could, but Noobs don't even know how to buy items.</p>
<p>An obvious piece of preqrequisite information for making such a bot is knowing what sorts of items are worth picking up. There are Normal, Magic, Rare, and Set items:</p>
<ul>
<li>Set items always belong to some famous dead person, so they always begin with a word that ends in "<strong>'s</strong>" (e.g. <strong>Andrew's</strong>). No other items are special enough to begin this way.</li>
<li>Rare items always have names that are two words long.</li>
<li>Magic items always have names that are between two and four words long, inclusive. If, and only if, a Magic item has more than two words in its name, then the last two words are "<strong>of [something]</strong>" (e.g. <strong>of Doom</strong>).</li>
<li>If the first word is "<strong>Damaged</strong>", the item is a Normal item. Furthermore, any item that could not possibly be Magic, Rare, or Set must also be Normal. No other items are Normal.</li>
<li>You may not have played Diablo, but hopefully you still know that a "word" is a maximal substring of non-space characters. Also, letter case is irrelevant.</li>
</ul>
<p>You have a list of $N$ ($1 \leq N \leq 1000$) item names, and you need to be able to classify these items as accurately as possible. It may not be possible to assign a unique type to each item, but as long as it's not Normal, surely you'll want it. Every item name is a string of no more than 100 characters, containing only alphabetic characters, spaces, and apostrophes. Every name begins and ends with a non-space character.</p>
<h3>Input</h3>
<p>First line: 1 integer, $N$</p>
<p>Next $N$ lines: The name of the $i$th item, for $i = 1..N$</p>
<h3>Output</h3>
<p>$N$ lines: The type of the $i$th item (one of "Normal", "Set", "Magic", or "Rare"), or "Not sure, take anyways" (without quotes) if the item's type cannot be determined, but is known not to be Normal, for $i = 1..N$</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">7<br>Somebody's Something of Whatever<br>stone of jordan<br>Wirt's Leg<br>FLAMING TURNIP<br>Damaged Goods<br>Sword<br>Fish shaped volatile organic compounds</span>

<strong>Output:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">Set<br>Magic<br>Set<br>Not sure, take anyways<br>Normal<br>Normal<br>Normal</span>&nbsp;</pre>
<pre><strong>Explanation of Sample:</strong></pre>
<p>The first and third items begin with possessives, so they must be Set items. The second item is three words long, and ends in "of [something]" so it must be Magic. The fourth item could be either Rare or Magic. The fifth item begins with "Damaged" so it's Normal. The last two items don't fit the descriptions of Set, Rare, or Magic, so they must be Normal also.</p>