## ��Ŀ����
Informational problems make us better.

## ��Ŀ����
������������ $\{a_n\}$��$\{b_n\}$ ������ȨֵΪ
$$\operatorname{unval}(a,b)=\sum_{i=1}^nb_i(b_i-a_i)$$

�ָ���һ������ $\{a_n\}$�������� $\operatorname{unval}(a,b)$ ��С�ĵ����������� $\{b\}$��ֻ����� $\operatorname{unval}(a,b)$ ��ֵ���ɡ�

ע�⣬$\{b\}$ �е�Ԫ�ز�һ��ҪΪ������

## �����ʽ
��һ��һ�������� $n$��

�ڶ��� $n$ ��������ʾ $a_i$��

## �����ʽ
һ��һ���𰸡�

```input1
5
1 2 3 4 5
```

```output1
-13.7500000
```

```input2
10
1000 1 2 8 9 5 4 1000 -40 1000
```

```output2
-403015.7500000
```

## ��ʾ
��ʾ������㲻��������⣬�������� [APJifengc](/user/279652)��
***

���� 1 ���ͣ�ʹ������Ȩֵȡ����Сֵ�� $\{b\}$ Ϊ `0.5 1 1.5 2 2.5`��

***
���ݷ�Χ��Լ����
$$
\newcommand{\arraystretch}{1.5}
\begin{array}{c|c|c|c}\hline\hline
\textbf{Subtask} & \bm{n}\le & \textbf{��ֵ} & \textbf{��������}\\\hline
\textsf{1} & 100 & 10 & \textbf{��} \\\hline
\textsf{2} & 10^6 & 5 & \{a\}\textbf{ ȫ�����} \\\hline
\textsf{3} & 10^6 & 5 & \{a\}\textbf{ ��������} \\\hline
\textsf{4} & 10^4 & 30 & \textbf{��} \\\hline
\textsf{5} & 10^6 & 50 & \textbf{��}
\\\hline\hline
\end{array}
$$

����ȫ�����ݣ��� $1\le n\le 10^6$��$|a_i|\le 10^3$��

***

���ֹ���

����ʹ�� Special Judge�������Ĵ��� $pans$����׼���� $cans$�����㽫���
$$\min\Bigg\{100,\Bigg\lfloor\dfrac{0.1}{\min\Big\{|pans-cans|,\Big|\dfrac{|pans-cans|}{cans}\Big|\Big\}}\Bigg\rfloor\Bigg\}$$
�֡�

**ÿ�� Subtask ���������**����ȡ Subtask �ڵ÷���С����Ϊ Subtask �÷֡�

