## Description

<div><p>Pasha loves his phone and also putting his hair up... But the hair is now irrelevant.</p><p>Pasha has installed a new game to his phone. The goal of the game is following. There is a rectangular field consisting of <span class="tex-span"><i>n</i></span> row with <span class="tex-span"><i>m</i></span> pixels in each row. Initially, all the pixels are colored white. In one move, Pasha can choose any pixel and color it black. In particular, he can choose the pixel that is already black, then after the boy's move the pixel does not change, that is, it remains black. Pasha loses the game when a <span class="tex-span">2 × 2</span> square consisting of black pixels is formed. </p><p>Pasha has made a plan of <span class="tex-span"><i>k</i></span> moves, according to which he will paint pixels. Each turn in his plan is represented as a pair of numbers <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span>, denoting respectively the row and the column of the pixel to be colored on the current move.</p><p>Determine whether Pasha loses if he acts in accordance with his plan, and if he does, on what move the <span class="tex-span">2 × 2</span> square consisting of black pixels is formed.</p></div><div class="input-specification"><p>The first line of the input contains three integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of rows, the number of columns and the number of moves that Pasha is going to perform. </p><p>The next <span class="tex-span"><i>k</i></span> lines contain Pasha's moves in the order he makes them. Each line contains two integers <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>j</i> ≤ <i>m</i></span>), representing the row number and column number of the pixel that was painted during a move.</p></div><div class="output-specification"><p>If Pasha loses, print the number of the move when the <span class="tex-span">2 × 2</span> square consisting of black pixels is formed.</p><p>If Pasha doesn't lose, that is, no <span class="tex-span">2 × 2</span> square consisting of black pixels is formed during the given <span class="tex-span"><i>k</i></span> moves, print <span class="tex-span">0</span>.</p></div>


## Input

<p>The first line of the input contains three integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of rows, the number of columns and the number of moves that Pasha is going to perform. </p><p>The next <span class="tex-span"><i>k</i></span> lines contain Pasha's moves in the order he makes them. Each line contains two integers <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>j</i> ≤ <i>m</i></span>), representing the row number and column number of the pixel that was painted during a move.</p>


## Output

<p>If Pasha loses, print the number of the move when the <span class="tex-span">2 × 2</span> square consisting of black pixels is formed.</p><p>If Pasha doesn't lose, that is, no <span class="tex-span">2 × 2</span> square consisting of black pixels is formed during the given <span class="tex-span"><i>k</i></span> moves, print <span class="tex-span">0</span>.</p>


## Samples

```input1
2 2 4
1 1
1 2
2 1
2 2

```

```output1
4

```






```input2
2 3 6
2 3
2 2
1 3
2 2
1 2
1 1

```

```output2
5

```






```input3
5 3 7
2 3
1 2
1 1
4 1
3 1
5 3
3 2

```

```output3
0

```



