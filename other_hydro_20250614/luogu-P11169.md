## ��Ŀ����
![](bilibili:BV1qF4m157gc)

> Can you imagine find wakeless,like a satellite,in the black sky?
>
> Somewhere,like a star.
>
> We dream about things way beyond this atmosphere.
>
> At we're now,on the air.
>
> ����
>
> But I eventually evaporates in a blackhole��
>
> Will I just stick up there?����

## ��Ŀ����
�������³����е� $n$�������룩��������α�������������

```
Input n
For i := 1 to n
	is_not_prime[i] := 0
cntp := 0
counter := 0
For i := 2 to n {
	If is_not_prime[i] = 0 {
		cntp := cntp + 1
		primes[cntp] := i
	}
	For j := 1 to cntp {
		If i * primes[j] > n
			break
		is_not_prime[i * primes[j]] := 1
		If i Mod primes[j] > 0 // should be `If i Mod primes[j] = 0` in Sieve of Euler
			break
		counter := counter + 1
	}
}
Print cntp, counter
```
��ע��˴���**��������ɸ**�������ע�͹�����һ�С�

## �����ʽ
һ��һ�������������룬Ҳ���Ǹ����� $n$��

## �����ʽ
һ�������Ǹ���������α���������

```input1
100
```

```output1
50 30
```

```input2
9876543
```

```output2
4938272 3092277
```

```input3
998877665544332211
```

```output3
499438832772166106 312742219398875473
```

## ��ʾ
**��������������**�����Ҵ���������������ֻ�����õ���һ��������ǰһ��������ķ֣�����п����õ���������ķ֣���

## ���ݷ�Χ

| $\text{Subtask}$ | Լ������ | ��ֵ |
| :-----------: | :-----------: | :-----------: |
| $1$ | $n\leq 10^7$ |$10$|
| $2$ | $n\leq 10^9$ |$40$|
| $3$ | $n\leq 10^{18}$ |$50$|

���� $100\%$ �����ݣ����� $1\leq n\leq 10^{18}$��

