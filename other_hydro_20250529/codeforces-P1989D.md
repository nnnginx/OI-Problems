## Description

<div><p>You are playing a famous computer game (that just works) where you have various skills you can level up. Today, you focused on the "Smithing" skill. Your tactic is obvious: forging weapons from ingots and then melting them back to return the materials partially. For simplicity, every time you create an item, you get $1$ experience point, and every time you melt an item, you also get $1$ experience point.</p><p>There are $n$ classes of weapons you can forge and $m$ types of metal ingots.</p><p>You can create one weapon of the $i$-th class, spending $a_i$ ingots of metal of <span class="tex-font-style-it">the same type</span>. Melting a weapon of the $i$-th class (which you crafted earlier) returns you $b_i$ ingots of the type of metal <span class="tex-font-style-it">it was made of</span>.</p><p>You have $c_j$ metal ingots of the $j$-th type, and you know that you can craft a weapon of any class from any metal type. Each combination of a weapon class and a metal type can be used any number of times.</p><p>What is the maximum total amount of experience you can earn by crafting and melting weapons?</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($1 \le n, m \le 10^6$)&nbsp;！ the number of weapon classes and metal types.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^6$), where $a_i$ is the number of ingots you need to forge one weapon of the $i$-th class.</p><p>The third line contains $n$ integers $b_1, b_2, \dots, b_n$ ($0 \le b_i &lt; a_i$), where $b_i$ is the number of ingots you return by melting one weapon of the $i$-th class you forged earlier.</p><p>The fourth line contains $m$ integers $c_1, c_2, \dots, c_m$ ($1 \le c_j \le 10^9$)&nbsp;！ the number of ingots you have of the corresponding metal type.</p></div><div class="output-specification"><p>Print one integer&nbsp;！ the maximum total experience points you can gain by repeatedly forging and melting weapons.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($1 \le n, m \le 10^6$)&nbsp;！ the number of weapon classes and metal types.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^6$), where $a_i$ is the number of ingots you need to forge one weapon of the $i$-th class.</p><p>The third line contains $n$ integers $b_1, b_2, \dots, b_n$ ($0 \le b_i &lt; a_i$), where $b_i$ is the number of ingots you return by melting one weapon of the $i$-th class you forged earlier.</p><p>The fourth line contains $m$ integers $c_1, c_2, \dots, c_m$ ($1 \le c_j \le 10^9$)&nbsp;！ the number of ingots you have of the corresponding metal type.</p>

## Output

<p>Print one integer&nbsp;！ the maximum total experience points you can gain by repeatedly forging and melting weapons.</p>





```input1|
5 3
9 6 7 5 5
8 4 5 1 2
10 4 7
```




```input2|
3 4
10 20 20
0 0 0
9 10 19 20
```




```input3|
1 5
3
1
1000000000 1000000000 1000000000 1000000000 1000000000
```




```output1
12
```




```output2
8
```




```output3
4999999990
```



## Note

<p>In the first example, you can do the following: </p><ol> <li> craft one weapon of the $1$-st class from the $1$-st type of metal, spending $9$ ingots; </li><li> melt that weapon, returning $8$ ingots of the $1$-st metal type; </li><li> again, craft and melt one weapon of the $1$-st class from the $1$-st metal type; </li><li> craft and melt one weapon of the $3$-rd class from the $1$-st metal type; </li><li> craft and melt one weapon of the $3$-rd class from the $3$-rd metal type; </li><li> craft and melt one weapon of the $4$-th class from the $1$-st metal type; </li><li> craft and melt one weapon of the $5$-th class from the $3$-rd metal type; </li></ol> In the end you'll have $c = [2, 4, 2]$ ingots left. In total, you've crafted $6$ weapons and melted $6$ weapons, gaining $12$ experience points in total.
