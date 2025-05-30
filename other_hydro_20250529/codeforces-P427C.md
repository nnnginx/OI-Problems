## Description

<div><p>Your city has <span class="tex-span"><i>n</i></span> junctions. There are <span class="tex-span"><i>m</i></span> <span class="tex-font-style-bf">one-way</span> roads between the junctions. As a mayor of the city, you have to ensure the security of all the junctions.</p><p>To ensure the security, you have to build some police checkposts. Checkposts can only be built in a junction. A checkpost at junction <span class="tex-span"><i>i</i></span> can protect junction <span class="tex-span"><i>j</i></span> if either <span class="tex-span"><i>i</i> = <i>j</i></span> or the police patrol car can go to <span class="tex-span"><i>j</i></span> from <span class="tex-span"><i>i</i></span> and then come back to <span class="tex-span"><i>i</i></span>.</p><p>Building checkposts costs some money. As some areas of the city are more expensive than others, building checkpost at some junctions might cost more money than other junctions.</p><p>You have to determine the minimum possible money needed to ensure the security of all the junctions. Also you have to find the number of ways to ensure the security in minimum price and <span class="tex-font-style-bf">in addition in minimum number of checkposts</span>. Two ways are different if any of the junctions contains a checkpost in one of them and do not contain in the other.</p></div><div class="input-specification"><p>In the first line, you will be given an integer <span class="tex-span"><i>n</i></span>, number of junctions <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>. In the next line, <span class="tex-span"><i>n</i></span> space-separated integers will be given. The <span class="tex-span"><i>i</i><sup class="upper-index"><i>th</i></sup></span> integer is the cost of building checkpost at the <span class="tex-span"><i>i</i><sup class="upper-index"><i>th</i></sup></span> junction (costs will be non-negative and will not exceed <span class="tex-span">10<sup class="upper-index">9</sup></span>).</p><p>The next line will contain an integer <span class="tex-span"><i>m</i>&nbsp;(0 ≤ <i>m</i> ≤ 3·10<sup class="upper-index">5</sup>)</span>. And each of the next <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub>&nbsp;(1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>u</i> ≠ <i>v</i>)</span>. A pair <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub></span> means, that there is a one-way road which goes from <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>. There will not be more than one road between two nodes in the same direction.</p></div><div class="output-specification"><p>Print two integers separated by spaces. The first one is the minimum possible money needed to ensure the security of all the junctions. And the second one is the number of ways you can ensure the security modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div>


## Input

<p>In the first line, you will be given an integer <span class="tex-span"><i>n</i></span>, number of junctions <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>. In the next line, <span class="tex-span"><i>n</i></span> space-separated integers will be given. The <span class="tex-span"><i>i</i><sup class="upper-index"><i>th</i></sup></span> integer is the cost of building checkpost at the <span class="tex-span"><i>i</i><sup class="upper-index"><i>th</i></sup></span> junction (costs will be non-negative and will not exceed <span class="tex-span">10<sup class="upper-index">9</sup></span>).</p><p>The next line will contain an integer <span class="tex-span"><i>m</i>&nbsp;(0 ≤ <i>m</i> ≤ 3·10<sup class="upper-index">5</sup>)</span>. And each of the next <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub>&nbsp;(1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>u</i> ≠ <i>v</i>)</span>. A pair <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub></span> means, that there is a one-way road which goes from <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>. There will not be more than one road between two nodes in the same direction.</p>


## Output

<p>Print two integers separated by spaces. The first one is the minimum possible money needed to ensure the security of all the junctions. And the second one is the number of ways you can ensure the security modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p>


## Samples

```input1
3
1 2 3
3
1 2
2 3
3 2

```

```output1
3 1

```






```input2
5
2 8 0 6 0
6
1 4
1 3
2 4
3 4
4 5
5 1

```

```output2
8 2

```






```input3
10
1 3 2 2 1 3 1 4 10 10
12
1 2
2 3
3 1
3 4
4 5
5 6
5 7
6 4
7 3
8 9
9 10
10 9

```

```output3
15 6

```






```input4
2
7 91
2
1 2
2 1

```

```output4
7 1

```



