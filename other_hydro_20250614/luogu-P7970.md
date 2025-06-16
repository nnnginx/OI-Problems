## ��Ŀ����
��һ�� $N\times M$ ���������д� $0$ ��ʼ�������ϵ����±�š�

�� $i$ �У��� $j$ �еĸ����Ǻڸ��ҽ��� $i\text{ and }j=0$��

�����ڸ���ͨ���ҽ������Ƕ��Ǻڸ������ǿ��Ծ������ɸ���**�ڱ�**�ĺڸ񵽴

���� $Q$ �����Σ����Ͻ�Ϊ $(x_1,y_1)$�����½�Ϊ $(x_2,y_2)$������Ҫ����ÿ������������еĺڸ��γ��˶�����ͨ�顣

## �����ʽ
��һ�������������� $N,M,Q$�����������С��ѯ��������

������ $Q$ �У�ÿ�������ĸ����� $x_1,y_1,x_2,y_2$������ѯ�ʾ��Ρ�

## �����ʽ
����ÿ���������һ�У�����һ������������𰸡�

```input1
6 5 4
0 0 3 2
0 2 1 3
0 1 2 4
5 4 5 4
```

```output1
1
1
2
0
```

## ��ʾ
**���������͡�**

����Ϊ�������ĸ�ѯ�ʵ�ͼʾ��

![](https://api.tlx.toki.id/api/v2/problems/JIDPROGSepzakraFyFK27n5u3QV/render/sample-q1.png) ![](https://api.tlx.toki.id/api/v2/problems/JIDPROGSepzakraFyFK27n5u3QV/render/sample-q2.png) ![](https://api.tlx.toki.id/api/v2/problems/JIDPROGSepzakraFyFK27n5u3QV/render/sample-q3.png) ![](https://api.tlx.toki.id/api/v2/problems/JIDPROGSepzakraFyFK27n5u3QV/render/sample-q4.png)

**�����ݷ�Χ��**

**�������������ԡ�**

* Subtask 1��5 points����ֻ����һ�����ݣ����� $N = M=12$��$Q=3$��ÿ��ѯ�ʵ� $(x_1,y_1,x_2,y_2)$ ����Ϊ $(1,1,9,8)$��$(8,8,11,11)$ �� $(4,3,5,9)$��
* Subtask 2��11 points����$N,M,Q\le 200$��
* Subtask 3��10 points����$N,M,Q\le 2000$��$x_1=x_2$��
* Subtask 4��20 points����$N,M,Q\le 2000$��
* Subtask 5��4 points����$x_1=x_2=0$��
* Subtask 6��6 points������֤����ÿ��ѯ�ʴ������� $k$ ʹ�� $x_1=x_2=2^k$��
* Subtask 7��29 points����$x_1=x_2$��
* Subtask 8��15 points�������������ơ�

�����������ݣ�$0\leq x_1\leq x_2<N\leq 10^9$��$0\leq y_1\leq y_2<M\leq 10^9$��$1\leq Q\leq 10^5$��

