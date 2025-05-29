## ��Ŀ����
Kotori is practicing making fireworks for the upcoming hanabi taikai$^1$. It takes her $n$ minutes to make a single firework, and as she is not really proficient in making fireworks, each firework only has a probability of $p \times 10^{-4}$ to be perfect.

After she finishes making a firework, she can just start making the next firework, or take $m$ minutes to light all the remaining fireworks finished before. If there is at least one perfect firework among the lit ones, she will be happy and go to rest. Otherwise, she will continue practicing. Can you tell her the minimum expected practicing time before she goes to rest if she takes the optimal strategy?

Notice that no matter how many fireworks remain, it always takes $m$ minutes to light them all.

$^1$ Hanabi taikai: Romaji of the Japanese word ``������``, which means the firework... err... party?

## �����ʽ
There are multiple test cases. The first line of the input contains an integer $T$ ($1 \le T \le 10^4$) indicating the number of test cases. For each test case:

The first and only line contains three integers $n$, $m$ and $p$ ($1 \le n, m \le 10^9$, $1 \le p \le 10^4$).

## �����ʽ
For each test case, output one line containing one number indicating the minimum expected practicing time.

Your answer will be considered correct if and only if the absolute or relative error does not exceed $10^{-4}$.

## ��Ŀ����
Kotori ���������̻���������һ֧�̻���Ҫ $n$ ���ӣ�ÿ֧�̻��� $p\times 10 ^ {-4}$ �ĸ����������ġ�

�� Kotori ������һ֧�̻�ʱ��������ѡ�����������Ҳ����ѡ���� $m$ ���ӵ�ȼ�����̻�������������������̻�����ô����ܿ��ģ���ͣ������Ϣ������������������̻������ܸ����������Ų����£����������೤ʱ�����ͣ������Ϣ��

ע�⣬�����Ѿ��������˶���֧�̻���Kotori ����Ҫ $m$ ���ӽ����ǵ�ȼ��

�������ݣ�$1\leq T, p\leq 10 ^ 4$��$1\leq n, m\leq 10 ^ 9$��Ҫ������������������ $10 ^ {-4}$��

```input1
3
1 1 5000
1 1 1
1 2 10000
```

```output1
4.0000000000
10141.5852891136
3.0000000000
```

