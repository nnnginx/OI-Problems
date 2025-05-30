## 题目描述
Harry Potter has damaged his magic wand in a fight with Lord Voldemort. He has decided to
get a new wand in Olivander's wand shop. On the floor of the shop, he saw ​N wands and ​N
wand boxes. The lengths of the wands are, respectively, $X_1$
,$X_2$
...​$X_n$
, and the box sizes are
$Y_1$
,​$Y_2$
...$Y_n$
. A wand of length ​X can be placed in a box of size ​Y if ​X ≤ ​Y
. Harry wants to know
if he can place all the wands in boxes so that each box contains exactly one wand.
Help him solve this difficult problem.

## 输入格式
The first line of input contains the positive integer ​N
(1 ≤ ​N
≤ 100), the number from the task.
The second line contains ​N
positive integers ​$X_i$
(1 ≤ ​$X_i$
≤ $10^9$​ ), the numbers from the task.
The third line contains ​N
positive integers ​$X_i$
(1 ≤ $X_i$
≤ $10^9$​​ ), the numbers from the task.

## 输出格式
If Harry can place all the wands in boxes, output “DA” (Croatian for yes), otherwise output
“NE” (Croatian for no).

## 题目大意
## 题意简述
有 $n$ 个棍子和 $n$ 个盒子，要求每个盒子里放的棍子的总长度不能超过盒子的高度。求是否有方案使得各个棍子都能放到任意一个盒子里。是输出 DA，否则输出 NE。（一个盒子里只能放一根棍子）
## 输入
输入共三行。

第一行，一个整数 $n$。

第二行， $n$ 个整数 $X_1,X_2,X_3,\dots,X_n$。其中第 $i$个数 $X_i$表示第 $i$根棍子的长度。

第三行， $n$个整数 $Y_1,Y_2,Y_3,\dots,Y_n$。其中第 $i$ 个数 $Y_i$ 表示第 $i$ 个盒子的高度。
## 输出
输出仅一行。即如果有能够将各个棍子都能放进任一盒子的方案输出 DA，否则输出 NE（输出不包括引号）。

## 样例解释
样例 $1$：哈利波特能够将所有棍子放进盒子里面。例如 $X_1\Rightarrow Y_3,X_2\Rightarrow Y_2,X_3\Rightarrow Y_1$。

样例 $2$：哈利波特不能够将所有棍子放进盒子里。
因为 $Y_2=2$，不能塞下任何一根棍子。

## 数据范围
对于 $60\%$ 的数据，保证 $n\leqslant9$。

对于 $100\%$ 的数据，保证 $n\leqslant100$，并且  $\forall i$，都满足 $X_i,Y_i\leqslant10^9$。

```input1
3
7 9 5
6 13 10
```

```output1
DA
```

```input2
4
5 3 3 5
10 2 10 10
```

```output2
NE
```

```input3
4
5 2 3 2
3 8 3 3
```

```output3
DA
```

## 提示
In test cases worth 60% of total points, it will hold ​N
≤ 9.

**Clarification of the first test case:**

Harry can place the wands in boxes. For example, he can place the wand of length 5 in a box of size
6, wand of length 7 in a box of size 13, and wand of length 9 in a box of size 10.

**Clarification of the second test case:**

Harry can’t place the wands in boxes because the box of size 2 can’t fit any of the wands.

