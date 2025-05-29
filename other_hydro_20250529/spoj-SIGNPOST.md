<h3>Examples</h3>
<pre><strong>Input:</strong>
The hero was deep inside the dragon's lair.
But he was not afraid; he knew what was coming.
Each dragon layer has some crossroads.
At each crossroad, one can go either left or right.
At each crossroad there is a signpost, indicating
what is to the left, and what is to the right, always
in the same format. One direction leads to the dragon.
If the hero, in full armour, went into the dragon's bedroom,
he would surely wake him up and become breakfast in bed.
So, the hero will definitely choose the other option.
The hero always reads this signpost into a single line,
by itself. Oh, here comes the first crossroads, 
thought the hero to himself.
Left to dragon. Right to princess.

Oh no, what is this sorcery!?
What heroes don't know, is that the signposts are cursed.
Whoever reads one, forgets which of the two options he 
definitely didn't want to pick. So the hero needs your help -
Every time he manages to read a signpost, tell him where he needs to go.
<strong>Output:</strong>
Right, to the princess!
</pre>
<pre><strong>Input:</strong>
The story contains at most 100 lines, none of which
are over 100 characters long.

The signposts are always read into a single, separate line,
and strictly follow the following format:
Left to x. Right to y.
Where x,y are non-empty strings made up of letters of
the english alphabet, one of them is 'dragon', and the other
is NOT 'dragon'. This line has no missing, or extra, spaces.
Notice that the above example is not a valid
signpost, as it violates 'one of x,y is dragon'.

Often, heroes just mentally prepare for the inevitable
signpost they will face.

Right to dragon. Left to princess.

Hm, on a real signpost the directions would probably be
the other way around, thought the hero. Wait, what is 
this before me!?

Left to dragon. Right to goodluck.
Left to youwillneedit. Right to dragon.

What is happening!? Where should I go???

Left to havefun. Right to dragon.
<strong>Output:</strong>
Right, to the goodluck!
Left, to the youwillneedit!
Left, to the havefun!
</pre>