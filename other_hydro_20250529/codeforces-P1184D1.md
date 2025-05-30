## Description

<div><p>The Third Doctor Who once correctly said that travel between parallel universes is "like travelling sideways". However, he incorrectly thought that there were infinite parallel universes, whereas in fact, as we now all know, there will never be more than 250.</p><p>Heidi recently got her hands on a multiverse observation tool. She was able to see all $n$ universes lined up in a row, with non-existent links between them. She also noticed that the Doctor was in the $k$-th universe.</p><p>The tool also points out that due to restrictions originating from the space-time discontinuum, the number of universes will never exceed $m$.</p><p>Obviously, the multiverse is unstable because of free will. Each time a decision is made, one of two events will randomly happen: a new parallel universe is created, or a non-existent link is broken.</p><p>More specifically, </p><ul>  <li> When a universe is created, it will manifest itself between any two adjacent universes or at one of the ends.  </li><li> When a link is broken, it could be cut between any two adjacent universes. After separating the multiverse into two segments, the segment <span class="tex-font-style-it">NOT</span> containing the Doctor will cease to exist. </li></ul><p>Heidi wants to perform a simulation of $t$ decisions. Each time a decision is made, Heidi wants to know the length of the multiverse (i.e. the number of universes), and the position of the Doctor.</p></div><div class="input-specification"><p>The first line contains four integers $n$, $k$, $m$ and $t$ ($2 \le k \le n \le m \le 250$, $1 \le t \le 1000$).</p><p>Each of the following $t$ lines is in one of the following formats: </p><ul> <li> "$1$ $i$" �� meaning that a universe is inserted at the position $i$ ($1 \le i \le l + 1$), where $l$ denotes the current length of the multiverse. </li><li> "$0$ $i$" �� meaning that the $i$-th link is broken ($1 \le i \le l - 1$), where $l$ denotes the current length of the multiverse. </li></ul></div><div class="output-specification"><p>Output $t$ lines. Each line should contain $l$, the current length of the multiverse and $k$, the current position of the Doctor.</p><p>It is guaranteed that the sequence of the steps will be valid, i.e. the multiverse will have length at most $m$ and when the link breaking is performed, there will be at least one universe in the multiverse.</p></div>

## Input

<p>The first line contains four integers $n$, $k$, $m$ and $t$ ($2 \le k \le n \le m \le 250$, $1 \le t \le 1000$).</p><p>Each of the following $t$ lines is in one of the following formats: </p><ul> <li> "$1$ $i$" �� meaning that a universe is inserted at the position $i$ ($1 \le i \le l + 1$), where $l$ denotes the current length of the multiverse. </li><li> "$0$ $i$" �� meaning that the $i$-th link is broken ($1 \le i \le l - 1$), where $l$ denotes the current length of the multiverse. </li></ul>

## Output

<p>Output $t$ lines. Each line should contain $l$, the current length of the multiverse and $k$, the current position of the Doctor.</p><p>It is guaranteed that the sequence of the steps will be valid, i.e. the multiverse will have length at most $m$ and when the link breaking is performed, there will be at least one universe in the multiverse.</p>

## Samples

```input1
5 2 10 4
0 1
1 1
0 4
1 2
```

```output1
4 1
5 2
4 2
5 3
```




## Note

<p>The multiverse initially consisted of 5 universes, with the Doctor being in the second.</p><p>First, link 1 was broken, leaving the multiverse with 4 universes, and the Doctor in the first.</p><p>Then, a universe was added to the leftmost end of the multiverse, increasing the multiverse length to 5, and the Doctor was then in the second universe.</p><p>Then, the rightmost link was broken.</p><p>Finally, a universe was added between the first and the second universe.</p>
