## ��Ŀ����

Farmer John's farm is made up of an $ n \times n $ grid of pastures, where each pasture contains one of two different types of grass. To specify these two types of grass, we use the characters ```(``` and ```)```, so for example FJ's farm might look like the following grid:

```
(())
)()(
)(((
))))
```

When Bessie the cow travels around the farm, it takes her $ A $ units of time to move from a pasture to an adjacent pasture (one step north, south, east, or west) with the same grass type, or $ B $ units of time to move to an adjacent pasture with a different grass type. Whenever Bessie travels from one pasture to a distant pasture, she always uses a sequence of steps that takes the minimum amount of time. Please compute the greatest amount of time Bessie will ever need to take while traveling between some pair of pastures on the farm.

��Ŀ���⣺����һ�� $ n \times n $ ��һ������ÿ��������һ���ַ���Ҫô�� ```(```��Ҫô�� ```)```��ÿ�����Ӻ������������ҵ��ĸ��������ڣ��������ڵ��������� $ x $ �� $ y $���� $ x $ �ߵ� $ y $ �Ĺ����У���� $ x $ �� $ y $ �е��ַ���ͬ������ $ A $ ��λʱ�䣬��� $ x $ �� $ y $ ���ַ���ͬ������ $ B $ ��λʱ�䡣����� $ S $ ���� $ T $ ��ʱ��Ϊ $ D(S,T) $������������������������� $ D(S,T) $��

## �����ʽ

��һ���������� $ n,a,b $��

������ $ n $ ��������� $ n\times n $ ������

## �����ʽ

һ������������ $D(S,T)$��

## ��������

```
3 1 2
(((
()(
(()
```

## �������

```
5
```

## ��ʾ

���Ͻǵ����½������ʱ��Ϊ $ 5 $�������ֵ��

## ���ݹ�ģ��Լ��

���� $100\%$ �����ݣ�$ 1 \leq n \leq 30 $��$ 1 \leq A \leq 1\times 10^6 $��$ 1 \leq B \leq 1\times 10^6 $��

## ��Ŀ��Դ

Silver

