## ��Ŀ����
��һ�������� $2n$ ���㣬����˳ʱ��˳����Ϊ $1,2,\dots 2n$��ÿ�����Ǻڵ���߰׵㣬һ���� $n$ ���ڵ�� $n$ ���׵㡣

���ǻ� $n$ ���߶����ӻ��ϵĵ㣬ʹ����������������

- ÿ����ǡ����һ���߶εĶ˵㡣
- ÿ���߶�����һ���ڵ��һ���׵㡣

����**�ཻ��**Ϊ�ཻ���߶ζ�����

����ÿ�������ɫ������ $n$ ���߶������ཻ����

## �����ʽ
��һ��һ������ $n$��

�ڶ���һ������Ϊ $2n$ ���ַ��� $S$���� $i$ ���ַ���ʾ�� $i$ �������ɫ��ÿ���ַ��� $\mathtt{B}$����ɫ���� $\mathtt{W}$����ɫ����

## �����ʽ
һ��������ʾ�����ཻ����

```input1
3
BBWWBW
```

```output1
2
```

```input2
5
BWBWBBWBWW
```

```output2
8
```

```input3
10
WBBBWBBWWBWWBWWBWBWB
```

```output3
41
```

```input4
16
WWWBWBBBBWWBWWBWWBBWWBBBWBBBWWBW
```

```output4
105
```

## ��ʾ
#### �������� 1

������ǰ���ͼ�����߶Σ���ô�ཻ������ $2$����һ���棬������ǰ���ͼ�����߶Σ���ô�ཻ���� $3$��Ȼ����������Ŀ�����е�������

![](https://cdn.luogu.com.cn/upload/image_hosting/7q5karom.png)

#### ���ݹ�ģ��Լ��

#### �������������ԡ�

- Subtask 1��4 pts����$n\le 8$��
- Subtask 2��21 pts����$n\le 300$��
- Subtask 3��10 pts����$n\le 2000$��
- Subtask 4��65 pts�������������ơ�

���� $100\%$ �����ݣ�$1\le n\le 2\times 10^5$����֤ $S$ �ĳ����� $2n$ ��ֻ���� $\mathtt{B}$ �� $\mathtt{W}$ �����ַ�����֤ $\mathtt{B}$ �� $\mathtt{W}$ ������ǡ�� $n$ �Ρ�

���� [JOI Open 2020](https://contests.ioi-jp.org/open-2020/index.html) T2 ��[���\�ε�](https://s3-ap-northeast-1.amazonaws.com/data.cms.ioi-jp.org/open-2020/monochrome/2020-open-monochrome-statement.pdf) / [Monochrome Points](https://s3-ap-northeast-1.amazonaws.com/data.cms.ioi-jp.org/open-2020/monochrome/2020-open-monochrome-statement-en.pdf)��

