## ��Ŀ����

����һ��ģ���⡣

���������Ǹ����� $x, y$ ���Ƕ����� Nim �� $x\otimes y$��

$$
x \otimes y = \operatorname {mex} \{ (a\otimes b) \oplus (a\otimes y) \oplus (x\otimes b) \mid 0\le a < x \wedge 0\le b < y  \}
$$

���� $\oplus$ ��������㣬$\operatorname{mex}$ �Ǽ����в����ڵ���С�Ǹ�������


## �����ʽ

��һ�������ĸ����� $T, \mathrm{SA}, \mathrm{SB}, \mathrm{SC}$��

Ϊ�˲���Ч�ʣ�ѯ������ $T$ ���ܴܺ�ʹ�����´�������ѯ�ʵ����룺

```cpp
unsigned int SA, SB, SC;
unsigned int rng() {
    SA ^= SA << 16;
    SA ^= SA >> 5;
    SA ^= SA << 1;
    unsigned int t = SA;
    SA = SB;
    SB = SC;
    SC ^= t ^ SA;
    return SC;
}
```

�ڽ����� $T$ ��ѯ���У��� $\mathrm{lastans}$ ���Ϊ $0$����˳����

```cpp
unsigned int x = rng() + lastans;
unsigned int y = rng();
lastans = nim_mul(x, y);
```

��˽��� $T$ ��ѭ����

## �����ʽ

���һ��һ����������ʾ���һ���Ĵ𰸡�

```input1
5 171380702 78283356 95463589
```

```output1
1145338263
```

## ���ݷ�Χ����ʾ

���ɵ����ݾ��� $2^{32}$ ��Χ���ڣ��ʱ�֤ $0\le x, y < 2^{32}$��

���������е� $T$ �ֱ�Ϊ $10, 1000, 3\times 10^4, 3\times 10^7$��

