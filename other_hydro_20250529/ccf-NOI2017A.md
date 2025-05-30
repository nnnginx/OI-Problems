## 题目描述

在人类智慧的山巅，有着一台字长为 $1048576$ 位的超级计算机，著名理论计算机科学家 P 博士正用它进行各种研究。
不幸的是，这天台风切断了电力系统，超级计算机无法工作，而 P 博士明天就要交实验结果了，只好求助于学过 OI 的你……

P 博士将他的计算任务抽象为对一个整数的操作。

具体来说，有一个整数 $x$ ，一开始为 $0$。

接下来有 $n$ 个操作，每个操作都是以下两种类型中的一种：

* `1` $a$ $b$ ：将 $x$ 加上整数 $a \cdot 2 ^ b$，其中 $a$ 为一个整数，$b$ 为一个非负整数

* `2` $k$ ：询问 $x$ 在用二进制表示时，位权为 $2 ^ k$ 的位的值（即这一位上的 $1$ 代表 $2 ^ k$ ）

保证在任何时候，$x \ge 0$。




## 输入格式

从标准输入读入数据。

输入的第一行包含四个正整数 $n, t_1, t_2, t_3$，$n$ 的含义见题目描述，$t_1, t_2, t_3$ 的具体含义见子任务。

接下来 $n$ 行，每行给出一个操作，具体格式和含义见题目描述。

同一行输入的相邻两个元素之间，用恰好一个空格隔开。


## 输出格式

输出到标准输出。

对于每个询问操作，输出一行，表示该询问的答案（$0$ 或 $1$）。
对于加法操作，没有任何输出。


```input1
10 3 1 2
1 100 0
1 2333 0
1 -233 0
2 5
2 7
2 15
1 5 15
2 15
1 -1 12
2 15
```

```output1
0
1
0
1
0
```

## 数据范围与提示

#### 子任务

在所有测试点中，$1 \le t_1 \le 3, 1 \le t_2 \le 4, 1 \le t_3 \le 2$。
不同的 $t_1, t_2, t_3$ 对应的特殊限制如下：

* 对于 $t_1 = 1$ 的测试点，满足 $a = 1$

* 对于 $t_1 = 2$ 的测试点，满足 $|a| = 1$

* 对于 $t_1 = 3$ 的测试点，满足 $|a| \le 10 ^ 9$

* 对于 $t_2 = 1$ 的测试点，满足 $0 \le b,k \le 30$

* 对于 $t_2 = 2$ 的测试点，满足 $0 \le b,k \le 100$

* 对于 $t_2 = 3$ 的测试点，满足 $0 \le b,k \le n$

* 对于 $t_2 = 4$ 的测试点，满足 $0 \le b,k \le 30 n$

* 对于 $t_3 = 1$ 的测试点，保证所有询问操作都在所有修改操作之后

* 对于 $t_3 = 2$ 的测试点，不保证询问操作和修改操作的先后顺序

本题共 25 个测试点，每个测试点 4 分。各个测试点的数据范围如下：


  <!-- BEGIN: Migrated markdown table -->

| 测试点编号 | $n \le$ | $t_1$ | $t_2$ | $t_3$ |
|:-:|:-:|:-:|:-:|:-:|
| $1$ | $10$ | $3$ | $1$ | $2$ |
| $2$ | $100$ | $3$ | $2$ | $2$ |
| $3$ | $2000$ | $3$ | $2$ | $2$ |
| $4$ | $4000$ | $1$ | $3$ | $2$ |
| $5$ | $6000$ | $3$ | $3$ | $1$ |
| $6$ | $8000$ | $2$ | $3$ | $2$ |
| $7$ | $9000$ | $3$ | $4$ | $2$ |
| $8$ | $10000$ | $3$ | $3$ | $2$ |
| $9$ | $30000$ | $3$ | $4$ | $2$ |
| $10$ | $50000$ | $3$ | $4$ | $1$ |
| $11$ | $60000$ | $3$ | $3$ | $2$ |
| $12$ | $65000$ | $2$ | $4$ | $2$ |
| $13$ | $70000$ | $3$ | $4$ | $2$ |
| $14$ | $200000$ | $3$ | $4$ | $2$ |
| $15$ | $300000$ | $2$ | $4$ | $2$ |
| $16$ | $400000$ | $3$ | $4$ | $2$ |
| $17$ | $500000$ | $3$ | $3$ | $2$ |
| $18$ | $600000$ | $3$ | $4$ | $2$ |
| $19$ | $700000$ | $3$ | $4$ | $2$ |
| $20$ | $800000$ | $1$ | $4$ | $2$ |
| $21$ | $900000$ | $2$ | $4$ | $2$ |
| $22$ | $930000$ | $3$ | $3$ | $2$ |
| $23$ | $960000$ | $3$ | $4$ | $1$ |
| $24$ | $990000$ | $3$ | $3$ | $2$ |
| $25$ | $1000000$ | $3$ | $4$ | $2$ |

<!-- Migrated from original HTML table:
<table class="ui celled center aligned table">  <thead>  <tr>  <th rowspan="1"> 测试点编号 </th>  <th rowspan="1"> $n \le$ </th> 
 <th rowspan="1"> $t_1$ </th>  <th rowspan="1"> $t_2$ </th>  <th rowspan="1"> $t_3$ </th>  </tr>  </thead>  <tbody>  <tr>  <td rowspan="1"> $1$ </td>  <td rowspan="1"> $10$ </td>  <td rowspan="3"> $3$ </td>  <td rowspan="1"> $1$ </td>  <td rowspan="4"> $2$ </td>  </tr>  <tr>  <td rowspan="1"> $2$ </td>  <td rowspan="1"> $100$ </td>  <td rowspan="2"> $2$ </td>  </tr>  <tr>  <td rowspan="1"> $3$ </td>  <td rowspan="1"> $2000$ </td>  </tr>  <tr>  <td rowspan="1"> $4$ </td>  <td rowspan="1"> $4000$ </td>  <td rowspan="1"> $1$ </td>  <td rowspan="3"> $3$ </td>  </tr>  <tr>  <td rowspan="1"> $5$ </td>  <td rowspan="1"> $6000$ </td>  <td rowspan="1"> $3$ </td>  <td rowspan="1"> $1$ </td>  </tr>  <tr>  <td rowspan="1"> $6$ </td>  <td rowspan="1"> $8000$ </td>  <td rowspan="1"> $2$ </td>  <td rowspan="4"> $2$ </td>  </tr>  <tr>  <td rowspan="1"> $7$ </td>  <td rowspan="1"> $9000$ </td>  <td rowspan="5"> $3$ </td>  <td rowspan="1"> $4$ </td>  </tr>  <tr>  <td rowspan="1"> $8$ </td>  <td rowspan="1"> $10000$ </td>  <td rowspan="1"> $3$ </td>  </tr>  <tr>  <td rowspan="1"> $9$ </td>  <td rowspan="1"> $30000$ </td>  <td rowspan="2"> $4$ </td>  </tr>  <tr>  <td rowspan="1"> $10$ </td>  <td rowspan="1"> $50000$ </td>  <td rowspan="1"> $1$ </td>  </tr>  <tr>  <td rowspan="1"> $11$ </td>  <td rowspan="1"> $60000$ </td>  <td rowspan="1"> $3$ </td>  <td rowspan="12"> $2$ </td>  </tr>  <tr>  <td rowspan="1"> $12$ </td>  <td rowspan="1"> $65000$ </td>  <td rowspan="1"> $2$ </td>  <td rowspan="5"> $4$ </td>  </tr>  <tr>  <td rowspan="1"> $13$ </td>  <td rowspan="1"> $70000$ </td>  <td rowspan="2"> $3$ </td>  </tr>  <tr>  <td rowspan="1"> $14$ </td>  <td rowspan="1"> $200000$ </td>  </tr>  <tr>  <td rowspan="1"> $15$ </td>  <td rowspan="1"> $300000$ </td>  <td rowspan="1"> $2$ </td>  </tr>  <tr>  <td rowspan="1"> $16$ </td>  <td rowspan="1"> $400000$ </td>  <td rowspan="4"> $3$ </td>  </tr>  <tr>  <td rowspan="1"> $17$ </td>  <td rowspan="1"> $500000$ </td>  <td rowspan="1"> $3$ </td>  </tr>  <tr>  <td rowspan="1"> $18$ </td>  <td rowspan="1"> $600000$ </td>  <td rowspan="4"> $4$ </td>  </tr>  <tr>  <td rowspan="1"> $19$ </td>  <td rowspan="1"> $700000$ </td>  </tr>  <tr>  <td rowspan="1"> $20$ </td>  <td rowspan="1"> $800000$ </td>  <td rowspan="1"> $1$ </td>  </tr>  <tr>  <td rowspan="1"> $21$ </td>  <td rowspan="1"> $900000$ </td>  <td rowspan="1"> $2$ </td>  </tr>  <tr>  <td rowspan="1"> $22$ </td>  <td rowspan="1"> $930000$ </td>  <td rowspan="4"> $3$ </td>  <td rowspan="1"> $3$ </td>  </tr>  <tr>  <td rowspan="1"> $23$ </td>  <td rowspan="1"> $960000$ </td>  <td rowspan="1"> $4$ </td>  <td rowspan="1"> $1$ </td>  </tr>  <tr>  <td rowspan="1"> $24$ </td>  <td rowspan="1"> $990000$ </td>  <td rowspan="1"> $3$ </td>  <td rowspan="2"> $2$ </td>  </tr>  <tr>  <td rowspan="1"> $25$ </td>  <td rowspan="1"> $1000000$ </td>  <td rowspan="1"> $4$ </td>  </tr>  </tbody>  </table>
-->

<!-- END: Migrated markdown table --> 

