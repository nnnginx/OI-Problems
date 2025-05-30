## 题目描述


Bob found a nice task in his old math book for children. It says:

There are $10$ children standing in a circle, $5$ of them stand next to a boy, and $7$ of them stand next to a girl. How is it possible?

Here is the solution to the task. If $4$ boys and $6$ girls stand like this: BGBGBGBGGG, there are $5$ children who stand next to a boy (here they are underlined: BGBGBGBGGG), and $7$ children who stand next to a girl $(BGBGBGBGGG).$

Now Bob wants to solve a generalized version of this task:

There are $n$ children standing in a circle, $x$ of them stand next to a boy, and $y$ of them stand next to a girl. How is it possible?

Help Bob by writing a program that solves the generalized task.



## 输入格式


The single line of the input contains three integers $n , x$ and $y (2 \le n \le 100 000$ ; $0 \le x , y \le n)$ .



## 输出格式


If there is a solution, output a string of length $n$ , describing the order of children in the circle. $Character ‘G'$ corresponds to a girl, character $‘B'$ corresponds to a boy. If there are several solutions, output any $of the_m.$

If there is no solution, output `Impossible`.



## 题目大意
### 题目描述

Bob在他那本给孩子们的旧数学书中找到了一个好任务。上面写着：

有 $10$ 个孩子站成一个圆圈，其中 $5$ 个站在一个男孩旁边， $7$ 个站在一个女孩旁边。如何解决这个任务？

这个任务的解决方案如下：如果 $4$ 个男孩和 $6$ 个女孩像这样站着：$bgbgbbggg$，那么有 555 个孩子站在一个男孩旁边（用粗体字标记：b**g**b**g**b**g**b**g**g**g**）， 777 个孩子站在一个女孩旁边（用粗体字标记：**b**g**b**g**b**g**bggg**）。

现在Bob想解决这个任务的广义版本：

有 $n$ 个孩子站在一个圆圈里，其中 $x$ 个孩子站在一个男孩旁边， $y$ 个孩子站在一个女孩旁边。如何解决这个任务？

请编写一个程序来帮助Bob解决这个任务。

### 输入格式
一行，包括三个整数 $n$ , $x$ , $y$ 。($2≤n≤100000$; $0≤x,y≤n$) 

### 输出格式
若有解，输出一个长度为 $n$ 的字符串，描述圆中元素的顺序。每个字符 $G$ 对应一个女孩，字符 $B$ 对应一个男孩。如果有多个解决方案，则输出其中任意一种。
如果没有解决方案，输出```'Impossible'```
。（不包括引号）


```input1
10 5 7

```

```output1
BGBGBGBGGG

```

```input2
10 3 8

```

```output2
Impossible

```

## 提示
Time limit: 2 s, Memory limit: 256 MB. 



