## ��Ŀ����
[ͼ�齱����](https://amturing.acm.org/)��

## ��Ŀ����
������������hzhwcmhf ��ĸ� VFleaKing ����һ���⣺

����һ������Ϊ $n$ ���ַ��� $s$�����ж��ٸ���ͬ�ĳ���Ϊ $l$ �������Ӵ���

�����ַ�������Ϊ�ǲ�ͬ�ĵ��ҽ���ĳ��λ���ϵ��ַ���ͬ��

VFleaKing һ�������ⲻ�� Hash ������ô�����ǹ���д�˹�ϣ + ����

�� hzhwcmhf ���������Ȼ֪����������Ǻ�׺����� height �� $< l$ �ĸ��� +1�����Ǻ�׺�Զ����ϴ���ĳ���������� $l$ �Ľ����������Ǻ�׺�����Ϊ $l$ �Ľ���������

���� hzhwcmhf ��Ŀ��˿� VFleaKing ��������ʾ�ǳ����������뿨������

VFleaKing ʹ�õ����ֵ����ϣ�������������£�

```cpp
u64 val = 0;
for (int i = 0; i < l; i++)
    val = (val * base + s[i] - 'a') % MOD;
```

u64 ���޷��� int64����Χ�� $[0, 2^{64})$��VFleaKing �� val ��Ȼ�����

base ��һ��������VFleaKing ��������������ֵ��

$\text{MOD}$ �� `int32` ��Χ�ڵ��������� $\text{MOD}$ �ķ�Χ�� $[0,2^{31})$�����Ǹ�������VFleaKing ��������� $base^l \bmod \text{MOD}$���� base �� $l$ �η����� $\text{MOD}$ ���������������ܷ����������г���Ϊ $l$ ���Ӵ��Ĺ�ϣֵ��

Ȼ�� VFleaKing ����ϣֵ����ȥ�أ�����ж��ٸ���ͬ�Ĺ�ϣֵ�����������Ϊ�����

���� VFleaKing ��ʶ�������ᱻ�ӣ����ǲ��������� $\text{MOD}$ ��������⡣���� $\text{MOD}$ ģ������ֵ����ͬ�ű���Ϊ����ͬ��

���㷨�� C++ ��������:

```cpp
typedef unsigned long long u64;
typedef pair<int, int> PII;
const int MaxN = 100000;
inline int hash_handle(
const char *s, const int &n, const int &l, const int &base,
const int &mod1, const int &mod2)
{
    int li_n;
    static PII li[MaxN];
    u64 hash_pow_l;
    u64 val;
    hash_pow_l = 1;
    for (int i = 1; i <= l; i++)
        hash_pow_l = (hash_pow_l * base) % mod1;
    li_n = 0;
    val = 0;
    for (int i = 0; i < l; i++)
        val = (val * base + s[i] - 'a') % mod1;
    li[li_n++].first = val;
    for (int i = l; i < n; i++)
    {
        val = (val * base + s[i] - 'a') % mod1;
        val = (val + mod1 - ((s[i - l] - 'a') * hash_pow_l) % mod1) % mod1; li[li_n++].first = val;
    }
    hash_pow_l = 1;
    for (int i = 1; i <= l; i++)
        hash_pow_l = (hash_pow_l * base) % mod2;
    li_n = 0;
    val = 0;
    for (int i = 0; i < l; i++)
        val = (val * base + s[i] - 'a') % mod2;
    li[li_n++].second = val;
    for (int i = l; i < n; i++)
    {
        val = (val * base + s[i] - 'a') % mod2;
        val = (val + mod2 - ((s[i - l] - 'a') * hash_pow_l) % mod2) % mod2;
        li[li_n++].second = val;
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

��һ�������ÿո�������� $n, l$��

�ڶ�����һ������Ϊ $n$ ���ַ�����ֻ�ܰ���Сд��ĸ��

��Ҫ��֤ $1 \le n \le 10^5, 1 \le l \le n$�����������ϸ�ʽ�� WA����Ҫ�ж����ַ����ܿ��ܵ����� WA��

## ��ʾ
���������Ϊ��SPJ ��������� $20$ �� base �� $20$ ��˫��ϣģ�����ұ�֤��Ϊ�������Ҳ����˻��ɵ���ϣ��ÿ��һ�� base ���ֹ�ϣ��ͻ�� 5 �֣�����Ϊ 100 �֡�

