## ��Ŀ����

����֪�� $A \operatorname{nand} B=\operatorname{not} (A \operatorname{and} B)$ �����������������λλ��Ϊ $k$������ $2 \operatorname{nand} 3,k=3$���� $2 \operatorname{nand} 3=\operatorname{not} (2 \operatorname{and} 3)=\operatorname{not} 2=5$��

����һ����������ÿ���㶼�е�Ȩ���������ϴ� $a$ �� $b$ �ķ���Ϊ $0$ ��·���ϵĵ��Ȩֵ˳�� $\operatorname{nand}$ �Ľ�������磺�� $2$ �ŵ㵽 $5$ �ŵ�˳�ξ��� $2\to 3\to 5$��Ȩֵ�ֱ�Ϊ $5,7,2,k=3$����ô���ս��Ϊ $0 \operatorname{nand} 5 \operatorname{nand} 7 \operatorname{nand} 2=7 \operatorname{nand} 7 \operatorname{nand} 2=0 \operatorname{nand} 2=7$�������������Ҫ֧�����²�����

1. `Replace a b`������ $a$��$1\le a\le n$����Ȩֵ��Ϊ $b$��
2. `Query a b`������� $a$ ���� $b$ �ķ��á�

���������һ������֧����Щ������

## �����ʽ

- ��һ�� $n,m,k$�����Ľڵ��������ܲ�������������λ����
- ������һ�� $n$ �����֣����α�ʾ�ڵ� $i$ ��Ȩֵ��
- ������ $n-1$ �У�ÿ���������� $a,b$��$1\le a,b\le n$����ʾ $a,b$ ����һ�����ߡ�
- ������ $m$ �У�ÿ��һ��������Ϊ���� $2$ �����֮һ��

## �����ʽ

- ���ڲ��� $2$ ÿ�����һ�У�����Ŀ������

```input1
3 3 3
2 7 3 
1 2
2 3
Query 2 3
Replace 1 3
Query 1 1
```

```output1
4
7
```

## ���ݹ�ģ��Լ��

���� $100\%$ �����ݣ�$n,m\le 10^5$��$k\le 32$��

