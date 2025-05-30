<p>It is Byteman’s birthday today. There are n children at his birthday party (including Byteman). The children are numbered from 1 to n. Byteman’s parents have prepared a big round table and they have placed n chairs around the table. When the children arrive, they take seats. The child number 1 takes one of the seats. Then the child number 2 takes the seat on the left. Then the child number 3 takes the next seat on the left, and so on. Finally the child number n takes the last free seat, between the children number 1 and n−1.  Byteman’s parents know the children very well and they know that some of the children will be noisy, if they sit too close to each other. Therefore the parents are going to reseat the children in a specific order. Such an order can be described by a permutation p1, p2, . . . , pn (p1, p2, . . . , pn are distinct integers from 1 to n) — child pi (for i = 2,3, . . . ,n) should sit on child pi−1’s left, and child p1 should sit on child pn’s left. To seat all the children in the given order, the parents must move each child around the table to the left or to the right some number of seats. For each child, they must decide how the child will move — that is, they must choose a direction of movement (left or right) and distance (number of seats). On the given signal, all the children stand up at once, move to the proper places and sit down. The reseating procedure throws the birthday party into a mess. The mess is equal to the total distance any child moves. The children can be reseated in many ways. The parents choose one with minimum mess. Help them to find such a way to reseat the children.

</p><h3>Input</h3>
<p>The first line of standard input contains one integer n (1 ≤ n ≤ 50000). The second line contains n integers p1, p2, . . . , pn, separated by single spaces. Numbers p1, p2, . . . , pn form a permutation of the set {1,2, . . . ,n} describing the desired order of the children.

</p><h3>Output</h3>
<p>The first and the only line of standard output should contain one integer: the minimum possible mess.

</p><h3>Example</h3>

<pre><b>Input:</b>
5
1 5 4 3 2

<b>Output:</b>
6
</pre>