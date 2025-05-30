## Description

<div><p>Warawreh created a great company called Nanosoft. The only thing that Warawreh still has to do is to place a large picture containing its logo on top of the company's building.</p><p>The logo of Nanosoft can be described as four squares of the same size merged together into one large square. The top left square is colored with red, the top right square is colored with green, the bottom left square is colored with yellow and the bottom right square is colored with blue.</p><p>An Example of some correct logos:</p><p><img class="tex-graphics" src="./30880/file/N5VuauHD.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>An Example of some incorrect logos:</p><p><img class="tex-graphics" src="./30880/file/sFccegOK.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>Warawreh went to Adhami's store in order to buy the needed picture. Although Adhami's store is very large he has only one picture that can be described as a grid of $n$ rows and $m$ columns. The color of every cell in the picture will be green (the symbol '<span class="tex-font-style-tt">G</span>'), red (the symbol '<span class="tex-font-style-tt">R</span>'), yellow (the symbol '<span class="tex-font-style-tt">Y</span>') or blue (the symbol '<span class="tex-font-style-tt">B</span>').</p><p>Adhami gave Warawreh $q$ options, in every option he gave him a sub-rectangle from that picture and told him that he can cut that sub-rectangle for him. To choose the best option, Warawreh needs to know for every option the maximum area of sub-square inside the given sub-rectangle that can be a Nanosoft logo. If there are no such sub-squares, the answer is $0$.</p><p>Warawreh couldn't find the best option himself so he asked you for help, can you help him?</p></div><div class="input-specification"><p>The first line of input contains three integers $n$, $m$ and $q$ $(1 \leq n , m \leq 500, 1 \leq q \leq 3 \cdot 10^{5})$ &nbsp;�� the number of row, the number columns and the number of options.</p><p>For the next $n$ lines, every line will contain $m$ characters. In the $i$-th line the $j$-th character will contain the color of the cell at the $i$-th row and $j$-th column of the Adhami's picture. The color of every cell will be one of these: {'<span class="tex-font-style-tt">G</span>','<span class="tex-font-style-tt">Y</span>','<span class="tex-font-style-tt">R</span>','<span class="tex-font-style-tt">B</span>'}.</p><p>For the next $q$ lines, the input will contain four integers $r_1$, $c_1$, $r_2$ and $c_2$ $(1 \leq r_1 \leq r_2 \leq n, 1 \leq c_1 \leq c_2 \leq m)$. In that option, Adhami gave to Warawreh a sub-rectangle of the picture with the upper-left corner in the cell $(r_1, c_1)$ and with the bottom-right corner in the cell $(r_2, c_2)$.</p></div><div class="output-specification"><p>For every option print the maximum area of sub-square inside the given sub-rectangle, which can be a NanoSoft Logo. If there are no such sub-squares, print $0$.</p></div>

## Input

<p>The first line of input contains three integers $n$, $m$ and $q$ $(1 \leq n , m \leq 500, 1 \leq q \leq 3 \cdot 10^{5})$ &nbsp;�� the number of row, the number columns and the number of options.</p><p>For the next $n$ lines, every line will contain $m$ characters. In the $i$-th line the $j$-th character will contain the color of the cell at the $i$-th row and $j$-th column of the Adhami's picture. The color of every cell will be one of these: {'<span class="tex-font-style-tt">G</span>','<span class="tex-font-style-tt">Y</span>','<span class="tex-font-style-tt">R</span>','<span class="tex-font-style-tt">B</span>'}.</p><p>For the next $q$ lines, the input will contain four integers $r_1$, $c_1$, $r_2$ and $c_2$ $(1 \leq r_1 \leq r_2 \leq n, 1 \leq c_1 \leq c_2 \leq m)$. In that option, Adhami gave to Warawreh a sub-rectangle of the picture with the upper-left corner in the cell $(r_1, c_1)$ and with the bottom-right corner in the cell $(r_2, c_2)$.</p>

## Output

<p>For every option print the maximum area of sub-square inside the given sub-rectangle, which can be a NanoSoft Logo. If there are no such sub-squares, print $0$.</p>

## Samples

```input1
5 5 5
RRGGB
RRGGY
YYBBG
YYBBR
RBBRG
1 1 5 5
2 2 5 5
2 2 3 3
1 1 3 5
4 4 5 5
```

```output1
16
4
4
4
0
```






```input2
6 10 5
RRRGGGRRGG
RRRGGGRRGG
RRRGGGYYBB
YYYBBBYYBB
YYYBBBRGRG
YYYBBBYBYB
1 1 6 10
1 3 3 10
2 2 6 6
1 7 6 10
2 1 5 10
```

```output2
36
4
16
16
16
```






```input3
8 8 8
RRRRGGGG
RRRRGGGG
RRRRGGGG
RRRRGGGG
YYYYBBBB
YYYYBBBB
YYYYBBBB
YYYYBBBB
1 1 8 8
5 2 5 7
3 1 8 6
2 3 5 8
1 2 6 8
2 1 5 5
2 1 7 7
6 5 7 5
```

```output3
64
0
16
4
16
4
36
0
```




## Note

<p>Picture for the first test:</p><p><img class="tex-graphics" src="./30880/file/UdLAGbvg.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>The pictures from the left to the right corresponds to the options. The border of the sub-rectangle in the option is marked with black, the border of the sub-square with the maximal possible size, that can be cut is marked with gray.</p>
