## ��Ŀ����

Bessie the cow is trying to type a balanced string of parentheses into her new laptop, but she is sufficiently clumsy (due to her large hooves) that she keeps mis-typing characters. Please help her by computing the minimum number of characters in the string that one must reverse (e.g., changing a left parenthesis to a right parenthesis, or vice versa) so that the string would become balanced. There are several ways to define what it means for a string of parentheses to be "balanced". Perhaps the simplest definition is that there must be the same total number of ```(``` and ```)```, and for any prefix of the string, there must be at least as many ```(``` as ```)```.

For example, the following strings are all balanced:

```
()
(())
()(()())
```

while these are not:

```
)(
())(
((())))
```

��Ŀ���⣺��������Ϊ $n$ ��һ���������У�ÿ���޸Ŀ����޸�һ��λ�õ����ţ����������Ϊ```(```�����޸�Ϊ```)```�����������Ϊ```)```�����޸�Ϊ```(```���������޸Ķ��ٸ�ʹ��ԭ�������кϷ���
���У�
�� ```()```�ǺϷ��ģ�
�� �� $A$ �ǺϷ��ģ��� $(A)$ �ǺϷ��ģ�
�� �� $A,B$ ���ǺϷ��ģ��� $AB$ �ǺϷ��ġ�

## �����ʽ

һ������Ϊ $n$ ���������С�

## �����ʽ

���ٵ��޸Ĵ�����

## ��������

```
())(
```

## �������

```
2
```

## ��ʾ

�޸�Ϊ```()()```�����к�ɫ���ֱ�ʾ�޸ĵ����š�

## ���ݹ�ģ��Լ��

���� $100\%$ ���������㣺$1 \leq n \leq 1\times 10^5$��

## ��Ŀ��Դ

Silver

