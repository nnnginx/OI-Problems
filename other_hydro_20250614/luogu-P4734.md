## ��Ŀ����
Byteasar the hacker has qualified for this year��s IHO, the International Hacking Olympiad. One of the tasks in the Olympiad involves competing against a system operator. There are $n$ computers numbered from $1$ to $n$,connected in a ring topology, i.e. computers $i$ and $i+1$ are connected $(for \ i = 1,...,n-1)$, and also computers $n$ and $1$ are connected.
The competition is performed as a game between the hacker and the system operator:
   - Byteasar moves first. Afterwards, the operator and Byteasar move alternately.
   - In his first move, Byteasar chooses any computer and hacks it (for instance,by exploiting some operating system vulnerabilities).
   - In his first move, the operator chooses any non-hacked computer and protects it (for instance, by installing latest security upgrades).
   - In all his following moves, Byteasar either (a) does nothing or (b) chooses any computer that is neither hacked nor protected and is directly linked to any hacked computer, and hacks it.
   - In all his following moves, the operator either (a) does nothing or (b) chooses any computer that is neither hacked nor protected and is directly linked to any protected computer, and protects it.
   - The game ends as soon as both have done nothing in two subsequent moves.

At the beginning of the game none of the computers are hacked or protected.
Every computer $i$ has a certain value viwhich specifies the value of the data which is stored on it. For each hacked computer $i$, Byteasar scores its value $v_i$. Byteasar is quite a good hacker, but has no idea of algorithms.
That is why he asks you to write a program that computes his maximum possible score, assuming that the operator plays optimally.

## �����ʽ
The first line of input contains a positive integer $n(n \ge 2)$, specifying the number of computers. The second line contains a sequence of $n$ integers $v_1,v_2,...,v_n(1 \le v_i \le 2000)$; number vispecifies the value of the data
stored on computer $i$.

## �����ʽ
In the first and only line of output your program should write one integer: Byteasar��s maximum possible score against an optimally playing operator.

## ��Ŀ����
### ��������

Byteasar ����˽�����ʺڿͰ���ƥ�˾����Ĳ����ʸ񡣾���������֮һ����ϵͳ����Ա�������д� $1$ �� $n$ ��ŵ� $n$ ̨��������Ի������ӣ�������� $i$ �� $i+1$ ���ӣ����� $i = 1,2,\dots,n-1$�����ر�أ������ $n$ �� $1$ Ҳ���ӡ�

��������Ǻڿͺ�ϵͳ����Ա֮�����Ϸ��

- Byteasar ���ߡ�֮�󣬲���Ա�� Byteasar �����ƶ���
- Byteasar �ĵ�һ����ѡ���κ�һ̨�������������кڿ͹�����
- �����ĵ�һ���У�����Աѡ���κ�δ���ڿ͹����ļ������������б�����
- �ڽ����������ж����У�Byteasar Ҫôʲô��������Ҫôѡ���κμ�û�б��ڿ͹���Ҳû���ܵ������ļ��������ֱ�����ӵ��κα��ڿ͹����ļ������Ȼ�������кڿ͹�����
- �ڽ����������ж����У�����ԱҪôʲô��������Ҫôѡ���κμ�û�б��ڿ͹���Ҳû���ܵ������ļ������ֱ�����ӵ��κ��ܱ����ļ������������б�����
- һ�������ڽ����������������ж�û�����κ����飬��Ϸ�ͽ����ˡ�

����Ϸ��ʼʱ��û���κ�һ̨���Ա��ڿ͹������ܵ�������

ÿ̨����� $i$ ����һ���ض���ֵ $v_i$����ֵָ���˴洢�����ϵ����ݵļ�ֵ��Byteasar ���ջ�õķ����������б��������ļ������ $v$ ֵ֮�͡�

��Ȼ Byteasar ��һ���ܺõĺڿͣ������㷨һ����֪���������Ϊʲô��Ҫ�����дһ���������������������ܷ������������Ա�����Ų��ԡ�

### �����ʽ
��һ���������һ�������� $n(n\ge 2)$��ָ����������������ڶ��а���һ������ $n$ ������������ $v_1,v_2,\dots,v_n(1\le v_i\le 2000)$��

### �����ʽ

������ĵ�һ�У�Ҳ��Ψһһ�У���ĳ���Ӧ�����һ��������Byteasar ��õ��ܵ÷ֵ����ֵ��

```input1
4
7 6 8 4
```

```output1
13
```

```input2
5
1 1 1 1 1
```

```output2
3
```

## ��ʾ
**Explanation to the examples:** In the first example, Byteasar in his first move should hack computer $2$(scoring $6$). The operator��s response will be protecting computer $3$. In the next move Byteasar can hack computer $1$ (scoring $7$). Finally, the operator will protect computer $4$.

�����������������޹أ������ο���

![PVIZHx.png](https://s1.ax1x.com/2018/07/05/PVIZHx.png)

