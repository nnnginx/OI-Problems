<p>The pride of the Asia-Pacific region is the newly constructed Great Circular Zoo. Situated on
a small Pacific island, it consists of a large circle of different enclosures, each containing its own
exotic animal as illustrated below.</p>
<img src="/content/john_jones:zoo1.jpg">
<p>You are in charge of public relations for the zoo, which means it is your job to keep people as
happy as possible. A busload of schoolchildren has just arrived, and you are eager to please them.
However, this is no easy task|there are animals that some children love, and there are animals
that some children fear. For example, little Alex loves monkeys and koalas because they are cute,
but fears lions because of their sharp teeth. On the other hand, Polly loves lions because of their
beautiful manes, but fears koalas because they are extremely smelly.</p>
<p>You have the option of removing some animals from their enclosures, so that children are not
afraid. However, you are worried that if you remove too many animals then this will leave the
children with nothing to look at. Your task is to decide which animals to remove so that as many
children can be made happy as possible.</p>
<p>Each child is standing outside the circle, where they can see five consecutive enclosures. You
have obtained a list of which animals each child fears, and which animals each child loves. A child
will be made happy if either at least one animal they fear is removed from their field of vision, or at least one animal they love is not removed from their field of vision.</p>
<p>For example, consider the list of children and animals illustrated below:</p>
<img src="/content/john_jones:zoo2.jpg">
<pre>-----------------------------------------------------------------------
|Child      |Enclosures Visible |Fears                |Loves          |
|Alex       |2, 3, 4, 5, 6      |Enclosure 4          |Enclosures 2, 6|
|Polly      |3, 4, 5, 6, 7      |Enclosure 6          |Enclosure 4    |
|Chaitanya  |6, 7, 8, 9, 10     |Enclosure 9          |Enclosures 6, 8|
|Hwan       |8, 9, 10, 11, 12   |Enclosure 9          |Enclosure 12   |
|Ka-Shu     |12, 13, 14, 1, 2   |Enclosures 12, 13, 2 |-              |
-----------------------------------------------------------------------
</pre>
<p>Suppose you remove the animals from enclosures 4 and 12. This will make Alex and Ka-Shu
happy, because at least one animal that they fear has gone. This will also keep Chaitanya happy,
since both enclosures 6 and 8 still contain animals that he loves. However, both Polly and Hwan
will be unhappy, since they cannot see any animals that they love but they can still see all the
animals that they fear. This arrangement therefore gives a total of three happy children.</p>
<p>Now suppose you put these animals back into their enclosures, and remove the animals from
enclosures 4 and 6 instead. Alex and Polly will be happy because the animals that they fear in
enclosures 4 and 6 have gone. Chaitanya will be happy because, even though animal 6 has gone,
he can still see the animal in enclosure 8 which he loves. Likewise, Hwan will be happy because
she can now see the animal in enclosure 12, which she loves. The only person unhappy will be
Ka-Shu.</p>
<p>Finally, suppose you put the animals back once more and then remove only the animal from
enclosure 13. Ka-Shu will now be happy since one animal that he fears has been removed, and
Alex, Polly, Chaitanya and Hwan will all be happy since they can all see at least one animal that
they love. Thus this arrangement gives five happy children, the largest number possible.</p>
<h3>Input</h3>
<p>Multiple test cases, the number of them will be given at the very first line.</p>
<p>For each test case:</p>
<p>The first line will be of the form N C, where N is the number of animal enclosures
(10 &lt;= N &lt;= 10 000) and C is the number of children (1 &lt;= C &lt;= 50 000). The enclosures are
numbered 1, 2, ...,N clockwise around the circle.</p>
<p>Following this will be C additional lines of input, where each line describes a single child. Each
of these lines will be of the form:</p>
<pre>E F L X1 X2 ... XF Y1 Y2 ... YL;</pre>
<p>where:</p>
<div align="justify">
    <ul>
        <li>
        E is the first enclosure that the child can see (1 &lt;= E &lt;= N). In other words, the child can see enclosures E, E + 1, E + 2, E + 3 and E + 4. Note that numbers larger than N wrap back around the circle, so if N = 14 and E = 13 then the child can see enclosures 13, 14, 1, 2 and 3.
        </li><li>
        F is the number of animals that the child fears, and L is the number of animals that the child loves.
        </li><li>
        Enclosures X1,...,XF contain the animals that the child fears (1&lt;=X1,...,XF&lt;=N).
        </li><li>
        Enclosures Y1,...,YL contain the animals that the child loves (1&lt;=Y1,...,YL&lt;=N).
        </li><li>
        No two of the integers X1,...,XF,Y1,...,YL are equal, and all of these integers describe
enclosures that the child can see.</li>
    </ul>
</div>
<p>Children will be listed in sorted order according to the first enclosure E (so the child with
lowest E will appear first and the child with largest E will appear last). Note that more than one
child may have the same first enclosure E.</p>
<h3>Output</h3>
<p>Output must consist of a single integer, giving the largest number of children that can be made
happy.</p>
<h3>Example</h3>
<pre><b>Sample Input:</b>
2
14 5
2 1 2 4 2 6
3 1 1 6 4
6 1 2 9 6 8
8 1 1 9 12
12 3 0 12 13 2
12 7
1 1 1 1 5
5 1 1 5 7
5 0 3 5 7 9
7 1 1 7 9
9 1 1 9 11
9 3 0 9 11 1
11 1 1 11 1
<b>Sample Output:</b>
5
6

<b>Explanation:</b>
<p>The first sample case is the example discussed earlier, in which all C = 5 children can be made
happy. The second sample case is an example in which it is impossible to make all C = 7 children
happy.</p>
</pre>
<b>Warning: large input/output data,be careful with certain languages</b>