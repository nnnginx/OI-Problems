<p>
One of the most fundamental data structure problems is
the dictionary problem: given a set <var>D</var> of words you want to
be able to quickly determine if any given query string <var>q</var> is
present in the dictionary <var>D</var> or not. Hashing is a well-known
solution for the problem. The idea is to create a function
<var>h</var> : Σ <sup>∗</sup> → [0..<var>n</var> − 1] from all strings to the integer range
0,1,..,<var>n</var> − 1, i.e. you describe a fast deterministic program
which takes a string as input and outputs an integer between
0 and <var>n</var>−1. Next you allocate an empty hash table <var>T</var> of size
<var>n</var> and for each word <var>w</var> in <var>D</var>, you set <var>T</var>[<var>h</var>(<var>w</var>)] = <var>w</var>. Thus, given a query string <var>q</var>, you only
need to calculate <var>h</var>(<var>q</var>) and see if <var>T</var>[<var>h</var>(<var>q</var>)] equals <var>q</var>, to determine if <var>q</var> is in the dictionary.
Seems simple enough, but aren’t we forgetting something? Of course, what if two words
in <var>D</var> map to the same location in the table? This phenomenon, called collision, happens
fairly often (remember the Birthday paradox: in a class of 24 pupils there is more than
50% chance that two of them share birthday). On average you will only be able to put
roughly
√<var>n</var>-sized dictionaries into the table without getting collisions, quite poor space
usage!
</p><p>A stronger variant is Cuckoo Hashing. The idea is to use two hash functions <var>h</var><sub>1</sub>
and <var>h</var><sub>2</sub>. Thus each string maps to two positions in the table. A query string <var>q</var> is now handled
as follows: you compute both <var>h</var><sub>1</sub>(<var>q</var>) and <var>h</var><sub>2</sub>(<var>q</var>), and if <var>T</var>[<var>h</var><sub>1</sub>(<var>q</var>)] = <var>q</var>, or <var>T</var>[<var>h</var><sub>2</sub>(<var>q</var>)] = <var>q</var>, you
conclude that <var>q</var> is in <var>D</var>. The name “Cuckoo Hashing” stems from the process of creating
the table. Initially you have an empty table. You iterate over the words <var>d</var> in <var>D</var>, and
insert them one by one. If <var>T</var>[<var>h</var><sub>1</sub>(<var>d</var>)] is free, you set <var>T</var>[<var>h</var><sub>1</sub>(<var>d</var>)] = <var>d</var>. Otherwise if <var>T</var>[<var>h</var><sub>2</sub>(<var>d</var>)] is
free, you set <var>T</var>[<var>h</var><sub>2</sub>(<var>d</var>)] = <var>d</var>. If both are occupied however, just like the cuckoo with other
birds’ eggs, you evict the word <var>r</var> in <var>T</var>[<var>h</var><sub>1</sub>(<var>d</var>)] and set <var>T</var>[<var>h</var><sub>1</sub>(<var>d</var>)] = <var>d</var>. Next you put <var>r</var> back
into the table in its alternative place (and if that entry was already occupied you evict
that word and move it to its alternative place, and so on). Of course, we may end up
in an infinite loop here, in which case we need to rebuild the table with other choices of
hash functions. The good news is that this will not happen with great probability even if
<var>D</var> contains up to <var>n</var>/2 words
</p><h3>Input</h3>
<p>On the first line of input is a single positive integer 1 ≤ <var>t</var> ≤ 50 specifying the number of
test cases to follow. Each test case begins with two positive integers 1 ≤ <var>m</var> ≤ <var>n</var> ≤ 10000
on a line of itself, <var>m</var> telling the number of words in the dictionary and <var>n</var> the size of the
hash table in the test case. Next follow <var>m</var> lines of which the <var>i</var>:th describes the <var>i</var>:th word
<var>d</var><sub><var>i</var></sub> in the dictionary <var>D</var> by two non-negative integers <var>h</var><sub>1</sub>(<var>d</var><sub><var>i</var></sub>) and <var>h</var><sub>2</sub>(<var>d</var><sub><var>i</var></sub>) less than <var>n</var> giving the two hash function values of the word <var>d</var><sub><var>i</var></sub>. The two values may be identical.



</p><h3>Output</h3>
<p>For each test case there should be exactly one line of output either containing the string
“successful hashing” if it is possible to insert all words in the given order into the
table, or the string “rehash necessary” if it is impossible.


</p><h3>Example</h3>

<pre><b>Input:</b>
2
3 3
0 1
1 2
2 0
5 6
2 3
3 1
1 2
5 1
2 5
<b>Output:</b>
successful hashing
rehash necessary
</pre>