## ��Ŀ����

Georg �и� MP3 Player��û���κβ��� $t$ ���Ӿͻ���������ʱ��������һ�����ͻ���û������״̬��������ı�Ƶ����ֻ����û������״̬�°������п��ܸı�Ƶ����MP3 ��Ƶ��Ϊ $0 \sim v_{max}$����������� $x$ Ƶ������ $x < v_{max}$��������״̬�°� `+`��$x$ �ͻ�� $1$���� $x>0$��������״̬�°� `-`��$x$ �ͻ�� $1$��Georg ������ MP3 �� $t$ �Ƕ��١�����ͨ��һ�β�������һ�¡�Ȼ������д�����Ĳ���˳������ͣ����Ƶ�� $v_2$��Ȼ��͸����ˣ���Ҫ����� $t$ �����ֵ�� $t$ �����ֵ������£���һ������ǰ��Ƶ�� $v_1$ ������������

## �����ʽ

��һ�У�$n,v_{max},v_2$��$n$ ��ʾ Georg ������ $n$ �Σ�

���� $n$ �У�ÿ�е�һ��Ϊ�ַ� $c$���ڶ���Ϊ���� $t_i$����ʾ Georg �� $t_i$ �밴���� $c$ ����

## �����ʽ

��� $t$ �����ֵ�� $t$ �����ֵ������£���һ������ǰ��Ƶ�� $v_1$ ������������

�� $t$ Ϊ���޴�ʱ������β��������ͣ�� $v_2$������� `infinity`��

```input1
6 4 3
- 0
+ 8
+ 9
+ 13
- 19
- 24
```
```output1
5 4
```

## ����˵�� 1

For $t=5$ the keys perform the following actions: `unlock, unlock, +, +, unlock, -`.
For any we would get $v_2 = 3$. Note that the output contains the largest possible $v_1$.
For the last two keystrokes will both be active, hence it will be impossible to have $v_2=3$.

```input2
3 10 10
+ 1
+ 2
+ 47
```
```output2
infinity
```
## ����˵�� 2

If $v_1 = 10$ then for any $t$ we'll have $v_2 = 10$.

## ���ݹ�ģ��Լ��

���� $40\%$ �����ݣ�$n \leq 4\times10^3$��

���� $70\%$ �����ݣ�$n \times v_{max}\leq 4\times 10^5$��

���� $100\%$ �����ݣ�$2\leq n\leq 10^5$��$2\leq v_{max}\leq 5\times10^3$��$0 < c_i < 2\times 10^9$��$0\leq v_2 \leq v_{max}$��$x_i\in\{\texttt{+}, \texttt{-} \}$��