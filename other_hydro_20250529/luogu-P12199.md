## 题目背景
[图灵奖官网](https://amturing.acm.org/)。

## 题目描述
这天天气不错，hzhwcmhf 神犇给 VFleaKing 出了一道题：

给你一个长度为 $n$ 的字符串 $s$，求有多少个不同的长度为 $l$ 的连续子串。

两个字符串被认为是不同的当且仅当某个位置上的字符不同。

VFleaKing 一看觉得这不是 Hash 的裸题么！于是果断写了哈希 + 排序。

而 hzhwcmhf 神犇心里自然知道，这题就是后缀数组的 height 中 $< l$ 的个数 +1，就是后缀自动机上代表的长度区间包含 $l$ 的结点个数，就是后缀树深度为 $l$ 的结点的数量。

但是 hzhwcmhf 神犇看了看 VFleaKing 的做法表示非常汗。于是想卡掉他。

VFleaKing 使用的是字典序哈希，其代码大致如下：

```cpp
u64 val = 0;
for (int i = 0; i < l; i++)
    val = (val * base + s[i] - 'a') % MOD;
```

u64 是无符号 int64，范围是 $[0, 2^{64})$。VFleaKing 让 val 自然溢出。

base 是一个常量，VFleaKing 会根据心情决定其值。

$\text{MOD}$ 是 `int32` 范围内的素数，即 $\text{MOD}$ 的范围是 $[0,2^{31})$，且是个素数。VFleaKing 还求出来了 $base^l \bmod \text{MOD}$，即 base 的 $l$ 次方除以 $\text{MOD}$ 的余数，这样就能方便地求出所有长度为 $l$ 的子串的哈希值。

然后 VFleaKing 给哈希值排序，去重，求出有多少个不同的哈希值，把这个数作为结果。

但是 VFleaKing 意识到这样会被坑，于是采用了两个 $\text{MOD}$ 来解决问题。两个 $\text{MOD}$ 模出来的值都相同才被认为是相同。

其算法的 C++ 代码如下:

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

hzhwcmhf 当然知道怎么卡啦！但是他想考考你。

## 输出格式
你需要输出一组数据使得 VFleaKing 的代码 WA 掉。我们会使用 Special Judge 检查你的结果的正确性。

输出文件共两行。

第一行两个用空格隔开的数 $n, l$。

第二行是一个长度为 $n$ 的字符串。只能包含小写字母。

需要保证 $1 \le n \le 10^5, 1 \le l \le n$，不符合以上格式会 WA。不要有多余字符，很可能导致你 WA。

## 提示
本题的评分为：SPJ 会随机生成 $20$ 个 base 和 $20$ 组双哈希模数，且保证均为质数，且不会退化成单哈希。每让一个 base 出现哈希冲突记 5 分，满分为 100 分。

