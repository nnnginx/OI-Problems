## ��Ŀ����
Today the company has $m$ tasks to complete. The $i-$th task need $x_i$ minutes to complete. Meanwhile, this task has a difficulty level $y_i$. The machine whose level below this task��s level $y_i$ cannot complete this task. If the company completes this task, they will get $(500\times x_i+2\times y_i)$ dollars.

The company has $n$ machines. Each machine has a maximum working time and a level. If the time for the task is more than the maximum working time of the machine, the machine can not complete this task. Each machine can only complete a task one day. Each task can only be completed by one machine.

The company hopes to maximize the number of the tasks which they can complete today. If there are multiple solutions, they hopes to make the money maximum.

## �����ʽ
The input contains several test cases.

The first line contains two integers $N$ and $M$. $N$ is the number of the machines.M is the number of tasks $(1 \leq N \leq 100000, 1\leq M\leq 100000)$.

The following $N$ lines each contains two integers $x_i(0<x_i<1440),y_i(0\leq yi\leq 100)$. $x_i$ is the maximum time the machine can work. $y_i$ is the level of the machine. 

The following $M$ lines each contains two integers $x_i(0<x_i<1440),y_i(0\leq y_i\leq 100)$. $x_i$ is the time we need to complete the task. $y_i$ is the level of the task.

## �����ʽ
For each test case, output two integers, the maximum number of the tasks which the company can complete today and the money they will get.

## ��Ŀ����
**����Ŀ������**

���칫˾�� $m$ ������Ҫ��ɡ��� $i$ ��������Ҫ $x_i$ ��������ɡ�ͬʱ�����������һ�����Ѽ��� $y_i$��������ڸ����񼶱� $y_i$ �Ļ����޷�����������������˾����������������ǽ���� $(500\times x_i+2\times y_i)$ ��Ԫ��

��˾�� $n$ ̨������ÿ̨�������������ʱ���һ��������������ʱ�䳬�������������ʱ�䣬��û����޷�����������ÿ̨����һ��ֻ�����һ������ÿ������ֻ����һ̨������ɡ�

��˾ϣ����󻯽������ǿ�����ɵ�����������������ڶ���������������ϣ��ʹ������󻯡�

**�������ʽ��**

��һ�а����������� $N$ �� $M$��$N$ �ǻ�����������$M$ ����������� $(1 \leq N \leq 100000, 1\leq M\leq 100000)$��

�������� $N$ ��ÿ�а����������� $x_i(0<x_i<1440),y_i(0\leq y_i\leq 100)$��$x_i$ �ǻ������Թ������ʱ�䡣$y_i$ �ǻ����ļ���

�������� $M$ ��ÿ�а����������� $x_i(0<x_i<1440),y_i(0\leq y_i\leq 100)$��$x_i$ ��������������ʱ�䡣$y_i$ ������ļ���

**�������ʽ��**

����ÿ��������������������������ֱ��ǹ�˾���������ɵ�����������������ǽ���õ����档

���������ڣ�ChatGPT��

```input1
1 2 
100 3 
100 2 
100 1
```

```output1
1 50004
```

