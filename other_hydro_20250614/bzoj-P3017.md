## ��Ŀ����

Farmer John usually brands his cows with a circular mark, but his branding iron is broken, so he instead must settle for branding each cow with a mark in the shape of a parenthesis ����```(```. He has two breeds of cows on his farm: Holsteins and Guernseys. He brands each of his cows with a parenthesis-shaped mark. Depending on which direction the cow is facing, this might look like either a left parenthesis or a right parenthesis.

FJ's  $ n $  cows are all standing in a row, each facing an arbitrary direction, so the marks on the cows look like a string of parentheses of length  $ n $ . Looking at this lineup, FJ sees a remarkable pattern: if he scans from left to right through just the Holsteins (in the order they appear in the sequence), this gives a balanced string of parentheses; moreover, the same is true for the Guernseys! To see if this is truly a rare event, please help FJ compute the number of possible ways he could assign breeds to his $n$ cows so that this property holds.

There are several ways to define what it means for a string of parentheses to be "balanced". Perhaps the simplest definition is that there must be the same total number of ```(``` and ```)```, and for any prefix of the string, there must be at least as many ```(``` as ```)```. For example, following strings are all balanced:

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

��Ŀ���⣺����һ������Ϊ $ n $ ���������У�ÿ��Ҫô��```(```��Ҫô��```)```������԰�ÿ��λ�õ����ű��Ϊ $ H $ �������Ǳ��Ϊ $ G $ ��Ҫ���ź�������������б��Ϊ $ H $ ����������һ���ǺϷ��ģ����б��Ϊ $ G $ ����������һ��Ҳ�ǺϷ�
�ġ�

���У�
�� ```()```�ǺϷ��ģ�
�� �� $ A $ �ǺϷ��ģ��� $ (A) $ �ǺϷ��ģ�
�� �� $ A,B $ ���ǺϷ��ģ��� $ AB $ �ǺϷ��ġ�
��ô��ͬ�ı�ŷ�ʽ�ж����֣��𰸶� $ 2012 $ ȡģ��

## �����ʽ

һ������Ϊ $ n $ ���������С�

## �����ʽ

��ͬ�ı�ŷ�ʽ�� $ 2012 $ ȡģ���ֵ��

## ��������

```
(())
```

## �������

```
6
```

## ��ʾ

```
(())
HHHH
(())
GGGG
(())
HGGH
(())
GHHG
(())
HGHG
(())
GHGH
```

## ���ݹ�ģ��Լ��

���� $100\%$ ���������㣺 $ 1 \leq n \leq 1\times 10^3 $ ��

## ��Ŀ��Դ

Silver

