<p>The local zoo has acquired a large open garden in which animals may freely move as in their natural
habitats and entertain visitors with their usual shenanigans.
</p><p>The most popular animals are monkeys. With their climbing and jumping and other skills, they delight
old and young visitors alike.
</p><p>One species of monkey has specialized in climbing tall trees and picking off coconuts. Another species
has specialized in breaking them open.
</p><p>There are N monkeys of the first type (numbered 1 through N) and M monkeys of the second type
(numbered 1 through M).
</p><p>Monkey k of the first type takes Ak seconds to find a good spot on the tree, after which it picks off its
first coconut. After that the monkey produces a new coconut every Bk seconds.
</p><p>Monkey k of the second type takes Ck seconds to find a good tool for opening the coconuts, after
which it opens its first coconut. After that the monkey opens another coconut every Dk seconds.
</p><p>Unfortunately, the second type of monkey is extremely aggressive so the two types may not be in the
garden at the same time. Therefore, zoo keepers will chase away the first type of monkeys as soon as
they have picked off all the coconuts. Similarly, if monkeys of the same type stay too long after opening
all the coconuts, fights will ensue. Because of that, zoo keepers will send them away as soon as they
have opened all the coconuts.
</p><p>The zoo keepers first arrive immediately after all coconuts have been picked, and again immediately
after the monkeys open them all. The time needed for monkeys to enter or leave the garden is also
negligibly small.
</p><p>Tomislav especially likes the second type of monkey, but can never guess when to arrive in order to see
them. Help him calculate the time when the second type arrives if he knows the total time that
monkeys spent in the garden, but does not know the number of coconuts in the garden.

</p><h3>Input</h3>
<p>The first line contains the integer T (1 ¡Ü T ¡Ü 1 000 000 000), the total time that monkeys spent in the
garden, in seconds.
</p><p>The next line contains the integer N (1 ¡Ü N ¡Ü 100), the number of monkeys of the first type.
</p><p>Each of the following N lines contains two integers Ak and Bk (1 ¡Ü Ak, Bk ¡Ü 1 000 000 000), how fast
monkey k of the first type is.
</p><p>The next line contains the integer M (1 ¡Ü M ¡Ü 100), the number of monkeys of the second type.
</p><p>Each of the following M lines contains two integers Ck and Dk (1 ¡Ü Ck, Dk ¡Ü 1 000 000 000), how fast
monkey k of the second type is.

</p><h3>Output</h3>
<p>Output the number of seconds between the arrival of the first type of monkeys and the arrival of the
second type.

</p><h3>Example</h3>

<pre><b>Input:</b>
20
2
3 2
1 3
3
3 1
4 1
5 1

<b>Output:</b>
13

</pre>