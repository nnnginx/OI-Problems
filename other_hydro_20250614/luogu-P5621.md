## ��Ŀ����
```cpp
������֪������ɯ�����һ�ɰ���
����zhengrunzhe
```

�����ڴ����$3$��ͻȻ�ҳ����ˣ�������װ���ڴ����ݽṹ�⡣

![����̸�](https://cdn.luogu.com.cn/upload/pic/70922.png)

## ��Ŀ����
�� $n$ �������ޣ�ÿ�����������������ֵ��health ��������energy ��������attack ��������defense �������� collapse �����ܡ�

����ɯ������ѡһֻ������չ���������������ɵ��˱�����$i$ ��ô�����ջ� `collapse[i]` �Ŀɰ�ֵ�����ڵ���ɯԽսԽ�£��������һֻ������ $j$ ��Ҫ���� `health[j]�� health[i]` , `energy[j]��energy[i]` , `attack[j]��attack[i]` , `defense[j]��defense[i]`��

���������ɯ����һ�����ܹ���õ����ɰ�ֵ��

## �����ʽ
��һ��һ��������$n$��

������$n$�У���$i+1$���������`health[i]`��`energy[i]`��`attack[i]`��`defense[i]`��`collapse[i]`�������ŵ� $i$ ֻ�����޵�����ֵ��

## �����ʽ
һ��һ���������������ɰ�ֵ�������ɱ����һֻ�����ޣ����𰸱�֤���ᳬ�� long long ��Χ��$2^{63}-1$����

```input1
5
1 9 3 6 233
0 8 3 7 666
-3 9 4 2 810
2 3 3 3 -100
1 8 8 9 603
```

```output1
1269
```

## ��ʾ

Subtask #1��$20$�֣��� 

$1\leq n\leq 100$��

Subtask #2��$20$�֣��� 

$1\leq n\leq 10000$��

Subtask #3��$60$�֣��� 

$1\leq n\leq 50000$��

���� $100\%$ �����ݣ����� $|\mathrm{health}_i|, |\mathrm{energy}_i|, |\mathrm{attack_i}|, |\mathrm{defense}_i| \le 10^5$��$| \mathrm{collapse}_i|\le 10^9$��

### ��Ŀ�ṩ�ߣ�[$\color{red}{zhengrunzhe}$](https://www.luogu.org/space/show?uid=14374)

