## Description

<div><p>A Christmas party in city S. had <span class="tex-span"><i>n</i></span> children. All children came in mittens. The mittens can be of different colors, but each child had the left and the right mitten of the same color. Let's say that the colors of the mittens are numbered with integers from 1 to <span class="tex-span"><i>m</i></span>, and the children are numbered from 1 to <span class="tex-span"><i>n</i></span>. Then the <span class="tex-span"><i>i</i></span>-th child has both mittens of color <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>The Party had Santa Claus ('Father Frost' in Russian), his granddaughter Snow Girl, the children danced around the richly decorated Christmas tree. In fact, everything was so bright and diverse that the children wanted to wear mittens of distinct colors. The children decided to swap the mittens so that each of them got one left and one right mitten in the end, and these two mittens were of distinct colors. All mittens are of the same size and fit all the children.</p><p>The children started exchanging the mittens haphazardly, but they couldn't reach the situation when each child has a pair of mittens of distinct colors. Vasily Petrov, the dad of one of the children, noted that in the general case the children's idea may turn out impossible. Besides, he is a mathematician and he came up with such scheme of distributing mittens that the number of children that have distinct-colored mittens was maximum. You task is to repeat his discovery. Note that the left and right mittens are different: each child must end up with one left and one right mitten.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> — the number of the children and the number of possible mitten colors (<span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 100</span>). The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ... <i>c</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> is the color of the mittens of the <span class="tex-span"><i>i</i></span>-th child (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>).</p></div><div class="output-specification"><p>In the first line, print the maximum number of children who can end up with a distinct-colored pair of mittens. In the next <span class="tex-span"><i>n</i></span> lines print the way the mittens can be distributed in this case. On the <span class="tex-span"><i>i</i></span>-th of these lines print two space-separated integers: the color of the left and the color of the right mitten the <span class="tex-span"><i>i</i></span>-th child will get. If there are multiple solutions, you can print any of them.</p></div>


## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> — the number of the children and the number of possible mitten colors (<span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 100</span>). The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ... <i>c</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> is the color of the mittens of the <span class="tex-span"><i>i</i></span>-th child (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>).</p>


## Output

<p>In the first line, print the maximum number of children who can end up with a distinct-colored pair of mittens. In the next <span class="tex-span"><i>n</i></span> lines print the way the mittens can be distributed in this case. On the <span class="tex-span"><i>i</i></span>-th of these lines print two space-separated integers: the color of the left and the color of the right mitten the <span class="tex-span"><i>i</i></span>-th child will get. If there are multiple solutions, you can print any of them.</p>


## Samples

```input1
6 3
1 3 2 2 1 1

```

```output1
6
2 1
1 2
2 1
1 3
1 2
3 1

```






```input2
4 2
1 2 1 1

```

```output2
2
1 2
1 1
2 1
1 1

```



