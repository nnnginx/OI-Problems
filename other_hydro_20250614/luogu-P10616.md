## ��Ŀ����
> ��In the casino, the cardinal rule is to keep them playing and to keep them coming back. The
longer they play, the more they lose, and in the end, we get it all.��  
> (from the 1995 film *Casino*)

## ��Ŀ����
Recent recessions have not been kind to entertainment venues, including the gambling industry. Competition is fierce among casinos to attract players with lots of money, and some have begun to offer especially sweet deals. One casino is offering the following: you can gamble as much as you want at the casino. After you are finished, if you are down by any amount from when you started, the casino will refund $x\%$ of your losses to you. Obviously, if you are ahead, you can keep all of your winnings. There is no time limit or money limit on this offer, but you can redeem it only once.

For simplicity, assume all bets cost $1$ dollar and pay out $2$ dollars. Now suppose $x$ is $20$. If you make $10$ bets in total before quitting and only $3$ of them pay out, your total loss is $3.2$ dollars. If $6$ of them pay out, you have gained $2$ dollars.

Given $x$ and the percentage probability $p$ of winning any individual bet, write a program to determine the maximum expected profit you can make from betting at this casino, using any gambling strategy.

## �����ʽ
The input consists of a single test case. A test case consists of the refund percentage $x (0 \leq x < 100)$ followed by the winning probability percentage $p (0 \leq p < 50)$. Both $x$ and $p$ have at most two digits after the decimal point.

## �����ʽ
Display the maximum expected profit with an absolute error of at most $10^{-3}$.

## ��Ŀ����
**����Ŀ������**

> ���ڶĳ����Ҫ�����������Ǽ����棬�����ǲ��ϻ������������Խ�ã����Խ�࣬���գ����ǻ�Ӯ��һ�С���  
> ��ժ�� 1995 ���Ӱ���ĳ�����

����ľ���˥�˶԰����Ĳ�ҵ���ڵ����ֳ��������Ѻá��ĳ�֮�侺�����ң���������Ǯ����ң�һЩ�ĳ���ʼ�ṩ�ر��ź���Żݡ�����һ���ĳ��ṩ�����Żݣ�������ڶĳ�������Ĳ����������ʱ�������ȿ�ʼʱ�����κν��ĳ����˻�����ʧ�� $x\%$����Ȼ�������ӮǮ�ˣ�����Ա������еĽ��𡣴��Ż�û��ʱ�����ƻ������ƣ�����ֻ�ܶ���һ�Ρ�

Ϊ�˼򻯣��������ж�ע�ĳɱ�Ϊ $1$ ��Ԫ����֧�� $2$ ��Ԫ�����ڼ��� $x$ �� $20$����������˳�ǰ�ܹ���ע $10$ �Σ�ֻ�� $3$ �λ�ʤ���������ʧ�� $3.2$ ��Ԫ����� $6$ �λ�ʤ�����׬�� $2$ ��Ԫ��

���� $x$ ��Ӯ���κε�����ע�ĸ��ʰٷֱ� $p$����дһ��������ȷ����������ĳ���ע���ܻ�õ������������ʹ���κζĲ����ԡ�

������һ����һ�Ĳ���������ɡ��������������˿�ٷֱ� $x (0 \leq x < 100)$�������Ӯ�ø��ʰٷֱ� $p (0 \leq p < 50)$��$x$ �� $p$ ��С������������λ���֡�

��ʾ����������󣬾��������� $10^{-3}$��

**�������ʽ��**

������һ����һ�Ĳ���������ɡ��������������˿�ٷֱ� $x (0 \leq x < 100)$�������Ӯ�ø��ʰٷֱ� $p (0 \leq p < 50)$��$x$ �� $p$ ��С������������λ���֡�

**�������ʽ��**

�������������󣬾��������� $10^{-3}$��

���������ڣ�[ChatGPT](https://chatgpt.com/)��


```input1
0 49.9
```

```output1
0.0
```

```input2
50 49.85
```

```output2
7.10178453
```

