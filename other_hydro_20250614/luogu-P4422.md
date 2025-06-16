## ��Ŀ����
Little Marica is making up a ~~nonsensical~~ unusual fairy tale and is telling to her grandfather who keeps interrupting her and asking her ~~stupid~~ intriguing questions.

In Marica��s fairy tale, $N$ children, denoted with numbers from $1$ to $N$ by their age (from the youngest denoted with $1$, to the oldest denoted with $N$), embarked on a train ride. The train leaves from the station $0$ and stops in order at stations $1, 2, 3 \dots$ to infinity.

Each of the following Marica��s statements is of the form: ��$At\  stop\ X, child\ A\ got\ out$��, where the order of these statements is completely arbitrary. In other words, it does not depend on the station order. Her grandfather sometimes asks a question of the form: ��$\textit{ Based on the statements so far, of the children denoted with a number greater than or equal}\allowbreak\textit{ to B, who is the youngest child that rode for Y or less stops?}$�� If at the moment the grandfather asks the question it hasn��t been said so far that a child is getting off the train, we assume that the child is riding for an infinite amount of stops.

Marica must give a correct answer to each of her grandfather��s questions, otherwise the grandfather will get mad and go to sleep. The answer must be correct in the moment when the grandfather asks the question, while it can change later given Marica��s new statements, but that doesn��t matter. Write a program that tracks Marica��s statements and answers her grandfather��s questions.

## �����ʽ
The first line of input contains the positive integers $N$ and $Q$ $(2 \le N, Q \le 2 \times 10^{5})$, the number of children and the number of statements. Each of the following $Q$ lines describes:

- either Marica��s statement of the form `M X A`, where $M$ denotes Marica, and $X$ and $A$ are positive integers $(1 \le X \le 10^{9}, 1 \le A \le N)$ from the task,
- or her grandfather��s question of the form `D Y B`, where $D$ denotes the grandfather, and $Y$ and $B$ are positive integers $(1 \le Y \le 10^{9}, 1 \le B \le N)$ from the task.

All of Marica��s statements correspond to different children and at least one line in the input is her grandfather��s question.

## �����ʽ
For each grandfather��s question, output the number of the required child in its own line. If no such child exists, output `-1`.

## ��Ŀ����
### ��������
С���￨���ڴ���һ�������ͯ�����¡���һ�߱���£�һ�߽�������үү����үү�ɸ����ˣ�����������һЩ��Ȥ�����⡣

��С���￨�Ĺ����У��� $N$ ������ֱ�Ϊ $1$~$N$ ��ĺ��ӣ���С��Ϊ $1$ �꣬����Ϊ $N$ �꣩����һ�죬����һ��˻𳵳�ȥ���С���·�����кö����վ���ֱ��� $0, 1, 2, 3 \dots$ ��š����е� $0$ վΪʼ��վ����ÿ��һ����վ����ͣ��������һ��ʱ�䡣ÿ�����Ӷ�������ѡ���Լ�ϲ���ĳ�վ�³���

С���￨ϲ�������������Ĺ��£����ڵ� $X$ վ������Ϊ $A$ ��ĺ����³��ˡ�������С���￨��ϰ�߷ǳ����ã����������µ�˳������ȫ����ġ����仰˵��$X$ �ǲ������ġ�үү֪��С���￨�Ļ�ϰ�ߣ�������ϲ��ʱ��ʱ��һЩ��Ȥ����������С������鷳�������������ģ���������ڵ��� $B$ ���ڵ� $Y$ վ�������� $Y$ վ����ǰ�³����������С���Ƕ�󣿡�

С���￨������ȷ�ش�үү�����⣬����үү����������˯����ֵ��ע����ǣ�С���￨�Ĵ𰸱����ڵ�ʱ����ȷ�ġ���ȻС���￨�����Ľ����п��ܻ�ı�����Ĵ𰸣����ⶼ���޹ؽ�Ҫ�ġ�

С���￨���Լ��Ļ�ϰ��ʮ�����Ρ����ڹ��µ�˳��������ң�С���￨�����޷���ȷ�ش�үү�����⡣�������ҵ��˴������㡣���С���￨��дһ�����򣬶�̬׷�����Ľ��������ش�үү�����⡣

### �����ʽ
����ĵ�һ�а������������� $N,Q\ (2 \le N,Q \le 2 \times 10^{5})$���ֱ�����ӵ�����������������

������ $Q$ �У�ÿ��һ����䡣���ĸ�ʽΪ `M X A` �� `D Y B`���ֱ����С���￨�Ľ�����үү�����⡣���� `M`��`D` Ϊ��д��ĸ��$X$��$Y$��$A$��$B$ $(1 \le X,Y \le 10^{9},1 \le A,B \le N)$ �ֱ�Ϊһ�����������������������������������Ŀ�б�֤������һ�� `D`��

### �����ʽ
����ÿһ������ `D` ���һ���𰸡���Ϊһ�����������үү�������޽⣬����� `-1`��


```input1
3 4
M 10 3
M 5 1
D 20 2
D 5 1

```

```output1
3
1

```

```input2
10 10
M 20 10
D 1 9
M 2 3
D 17 10
M 20 2
D 8 2
M 40 1
D 25 2
M 33 9
D 37 9

```

```output2
-1
-1
3
2
9
```

