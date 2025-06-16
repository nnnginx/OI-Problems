## ��Ŀ����

������������hzhwcmhf ��ĸ� VFleaKing ����һ���⣺

����һ������Ϊ $n$ ���ַ��� $s$ �����ж��ٸ���ͬ�ĳ���Ϊ $l$ �������Ӵ���

�����ַ�������Ϊ�ǲ�ͬ�ĵ��ҽ���ĳ��λ���ϵ��ַ���ͬ��

VFleaKing һ�������ⲻ�� Hash ������ô�����ǹ���д�˹�ϣ + ����

�� hzhwcmhf ���������Ȼ֪����������Ǻ�׺����� height �� $<L$ �ĸ��� $+ 1$�����Ǻ�׺�Զ����ϴ���ĳ���������� $l$ �Ľ����������Ǻ�׺�����Ϊ $l$ �Ľ���������
���� hzhwcmhf ��Ŀ��˿� VFleaKing ��������ʾ�ǳ����������뿨������
VFleaKing ʹ�õ����ֵ����ϣ�������������£�

```cpp
u64 val = 0;
for (int i = 0; i < l; i++)
    val = (val * base + s[i] - 'a') % MOD;
```

`u64` ���޷��� `int64`����Χ�� $[0, 2^{64})$��VFleaKing �� `val` ��Ȼ�����

`base` ��һ��������VFleaKing ��������������ֵ��

`Mod` ���� $10^9 + 7$��

VFleaKing ��������� `(base ^ l) % MOD`���� $base$ �� $l$ �η����� $Mod$ ���������������ܷ����������г���Ϊ $l$ ���Ӵ��Ĺ�ϣֵ��

Ȼ�� VFleaKing ����ϣֵ����ȥ�أ�����ж��ٸ���ͬ�Ĺ�ϣֵ�����������Ϊ�����

���㷨�� C++ �������£�

```cpp
typedef unsigned long long u64;
const int MaxN = 100000;
inline int hash_handle(const char *s, const int &n, const int &l, const int &base)
{
    const int Mod = 1000000007;
    u64 hash_pow_l = 1;
    for (int i = 1; i <= l; i++)
    hash_pow_l = (hash_pow_l * base) % Mod;
    int li_n = 0;
    static int li[MaxN];
    u64 val = 0;
    for (int i = 0; i < l; i++)
    val = (val * base + s[i] - 'a') % Mod;
    li[li_n++] = val;
    for (int i = l; i < n; i++)
    {
    val = (val * base + s[i] - 'a') % Mod;
    val = (val + Mod - ((s[i - l] - 'a') * hash_pow_l) % Mod) % Mod;
    li[li_n++] = val;
    }
    sort(li, li + li_n);
    li_n = unique(li, li + li_n) - li;
    return li_n;
}
```

hzhwcmhf ��Ȼ֪����ô�������������뿼���㡣

## �����ʽ

����Ҫ���һ������ʹ�� VFleaKing �Ĵ��� WA �������ǻ�ʹ�� Special Judge �����Ľ������ȷ�ԡ�

����ļ������С�

��һ�������ÿո�������� $n,l$��

�ڶ�����һ������Ϊ $n$ ���ַ�����ֻ�ܰ���Сд��ĸ��

��Ҫ��֤ $1\le n\le 10^5$��$1\le l\le n$�����������ϸ�ʽ�� WA����Ҫ�ж����ַ����ܿ��ܵ����� WA��
