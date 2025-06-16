## ��Ŀ����


A game of rock-paper-scissors is played by two players who simultaneously show out their moves: Rock, Paper , or Scissors. If their moves are the same, it's a draw. Otherwise, Rock beats Scissors, Paper beats Rock, and Scissors beat Paper .

The described procedure can be repeated many times. In this problem, two Finite State Machines (FSMs) will compete in a series of rounds. (Formally speaking, by FSMs we mean Moore machines in this problem. )

An FSM for playing rock-paper-scissors has finitely many states. Each state is described by the following: what move the FSM will make in the upcoming round, and what will be the new state in case of its opponent playing Rock, Paper , and Scissors.

![](/upload/images2/epic.png)

Fortunately, you know your opponent FSM -- the entire scheme except for one thing: you do not know the initial state of that FSM.

Your task is to design your own FSM to fight the given one. Your FSM must beat the opponent in at least $99\%$ of the first $1$ billion rounds. That's what we call an epic win!



## �����ʽ


The input file contains a description of the opponent FSM in the following format.

The first line contains an integer $n (1 \le n \le 100)$ -- the number of states in the FSM. States are numbered from $1$ to $n$ . Each of the following $n$ lines contains a description of the state: a character $c_{i}$ denoting the move made by FSM and integers $r_{i}, p_{i}, s_{i}$ denoting the next state in case of seeing Rock, Paper, or Scissors respectively $(c_{i}$ can be `R`, `P`, or `S`; $1 \le r_{i}, p_{i}, s_{i} \le n$



## �����ʽ


Write to the output the description of your FSM in the same format.

The initial state of your FSM is the first state.

The number of states may not exceed $50 000$ .



## ��Ŀ����
**����Ŀ������**

����Ϸ��ʯͷ�����ӡ������У�������ҷֱ�ͬʱ��ʾ�Լ����ж���*ʯͷ*��*����*����*��*��������˵��ж�һ�£���ƽ�֡�����*ʯͷ*���*����*��*��*���*ʯͷ*��*����*���*��*��

�������̿����ظ���Ρ��ڱ����У���̨����״̬�Զ�����Finite State Machines��FSM����������֡�ʯͷ�����ӡ�������׼ȷ��˵�������е� FSM ��ָ Moore ״̬������

һ̨������������桸ʯͷ�����ӡ������� FSM �������޵�״̬��ÿ��״̬��������Ϣ��������һ���б�̨�Զ��������ʾ�������ж����Լ�����һ���ж��ֳ�ʾ��*ʯͷ*��*����*����*��*ʱӦ��ת�Ƶ�����״̬��

![](https://cdn.luogu.com.cn/upload/image_hosting/j121iya3.png)

���˵��ǣ���֪�����ֵ� FSM����֪�������еĽṹ����Ψ����֪�����ĳ�ʼ״̬��

������������һ̨���Լ��� FSM ȥ�Ͷ��ֵĽ��ж�ս����� FSM ������ǰʮ�ڣ�${10}^9$�����д�ܶ������� $99 \%$ �֡��������ν��ʷʫ���ʤ����epic win����

**�������ʽ��**

�ӱ�׼�����ж���Զ��ֵ� FSM �������������¸�ʽ��

��һ��һ�������� $n$����ʾ FSM �е�״̬��������״̬�� $1$ �� $n$ ��š�

������ $n$ �У�ÿ������һ��״̬��һ���ַ� $c_i$ �Լ����������� $r_i, p_i, s_i$���ֱ��ʾ��״̬���ж����Լ������ֳ�ʾ��*ʯͷ*��*��*����*����*��Ӧ��ת�Ƶ�����״̬�ı�ţ����� $c_i$ ֻ����Ϊ $\{\texttt{R}, \texttt{P}, \texttt{S}\}$ ֮һ�����Ϊ $\texttt{R}$ ����ζ���ж�Ϊ��ʾ*ʯͷ*�����Ϊ $\texttt{P}$ ����ζ���ж�Ϊ��ʾ*��*�����Ϊ $\texttt{S}$ �ж�Ϊ��ʾ*����*��

**�������ʽ��**

������Ƶ� FSM ����ͬ��ʽ�������׼����С�

��� FSM �ĳ�ʼ״̬�� $1$ ��״̬��

��� FSM ��״̬������Ӧ���� $50000$��

**���������͡�**

��Ŀ�����е�ͼƬ��ʾ�����������и����Ķ��ֵ� FSM���Լ���������и�����һ����� FSM��

���ֵ� FSM ������ʾ*ʯͷ*��*��*��ȡ���ڳ�ʼ״̬��ֱ�������յ�*����*�����յ�*����*������������Ϊ�ı䡣

һ�ִ�������� FSM �ķ����ǳ�ʾ*��*��������ֳ�����ʾ*ʯͷ*��ֻ�������ʾ*��*����ʤ����������ֳ�ʾ��*��*��ͨ����ʾһ��*����*��������Ϊ�ı䣬���������ͻ������ʾ*ʯͷ*��Ȼ����Ϳ�����*��*������ˡ�

**�����ݷ�Χ��**

����ȫ�����ݣ�$1 \le n \le 100$��$c_i \in \{\texttt{R}, \texttt{P}, \texttt{S}\}$��$1 \le r_i, p_i, s_i \le n$��

**������Դ**��IOI 2021 ��ѵ�ӵ�һ������ҵ��PinkRabbit��

```input1
2
R 1 1 2
P 2 2 1

```

```output1
2
P 1 2 1
S 1 1 1

```

## ��ʾ
Time limit: 1 s, Memory limit: 256 MB. 



