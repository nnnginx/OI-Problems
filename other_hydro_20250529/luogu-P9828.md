## ��Ŀ����

At the Namomo Camp, a cute volunteer celebrates her birthday. Wowo buys her a huge cake. (The cake is so big that it has a 3D coordinate system inside.) There are $n$ cuboid shaped pieces of chocolates $\textbf{in}$ the cake. The $i$-th ($1\le i\le n$) chocolate consists of all points $(x,y,z)$ such that $min\_x[i]\le x\le max\_x[i], min\_y[i]\le y\le max\_y[i], min\_z[i]\le z\le max\_z[i]$. $min\_x,max\_x, min\_y,max\_y, min\_z, max\_z$ are $6$ arrays of integers. Chocolates may overlap or touch each other.

The volunteer wants to distribute the cake to the campers of the Namomo Camp. To show off his knife skill, Wowo decides to cut the cake into pieces by exactly $3$ cuts such that:

- The first cut is a plane whose equation is $x=a$ for some integer $a$ decided by Wowo.
- The second cut is a plane whose equation is $y=b$ for some integer $b$ decided by Wowo.
- The third cut is a plane whose equation is $z=c$ for some integer $c$ decided by Wowo.
- Each chocolate is $\textbf{touched}$ by at least one cut (i.e. each cuboid has a nonempty intersection with at least one plane).

Decide whether Wowo can cut the cake under the rules. If the answer is yes, output any possible solution.

## �����ʽ
The first line contains a single integer $n$ ($1\le n\le 100000$).

The $i$-th line of the next $n$ lines contains $6$ integers $min\_x[i],max\_x[i], min\_y[i],max\_y[i], min\_z[i], max\_z[i]$ ($-10^9\le min\_x[i],max\_x[i], min\_y[i],max\_y[i], min\_z[i], max\_z[i]\le 10^9$, $min\_x[i]<max\_x[i]$, $min\_y[i]<max\_y[i]$, $min\_z[i]< max\_z[i]$).

## �����ʽ
If Wowo can cut the cake under the rules, the first line of the output should contain ``YES`` and the second line should contain $3$ integers $a$, $b$ and $c$ ($-10^9\le a, b, c\le 10^9$). If Wowo cannot cut the cake under the rules, output only one line containing ``NO``.

## ��Ŀ����
��һ���޴�ĵ��⣬����������$n$����������״���ɿ�����ÿ���ɿ�����λ�������ĶԽ������궨�塣һ������ͨ������ƽ���и�������⣬ÿ��ƽ��ķ��̷ֱ���$x=a$��$y=b$��$z=c$������$a$��$b$��$c$��������Ŀ����ѡ��$a$��$b$��$c$����ÿ���ɿ������ٱ�һ���и�ƽ�津����

������һ������$n$��ʼ����ʾ�ɿ������������������$n$�У�ÿ�������������ֱ����ÿ���ɿ�������ά����ϵ�е���С�����$x$��$y$��$z$���ꡣ

���Ҫ����������������������и�ƽ�棬��һ�����``YES``���ڶ��������������$a$��$b$��$c$����������ڣ�ֻ���``NO``��

```input1
3
0 1 0 1 0 1
10 11 10 11 10 11
999999999 1000000000 999999999 1000000000 999999999 1000000000
```

```output1
YES
0 10 999999999
```

```input2
4
0 1 0 1 0 1
999999999 1000000000 0 1 0 1
0 1 999999999 1000000000 0 1
0 1 0 1 999999999 1000000000
```

```output2
YES
0 0 0
```

