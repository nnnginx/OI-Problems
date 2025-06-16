## ��Ŀ����
�����г��ֵ���ģ�[_lgswdn](https://www.luogu.com.cn/user/180652)

AK �� NOI ��lgd һ·�Ʋ��ɵ������ñ�����˹��Ҷӣ������� IOI ������

## ��Ŀ����
6ms ��lgd д�������һ���

```plain
�ɳ־û���ȷ��״̬AC�Զ��ֿ�ά���߶�ƽ���������Ż���С���������Ԥ������ͼ��Ī����˹����Ī�Ӵ����赸�����鼯��״��������ϯ��Ԥ����̬DP����FFT�����ʽ��Ԫ����������ָ�������ÿɳ־û����鼯�ϲ���С����ѭ�����ϲ�ͷDP
```
�㷨��AK �� IOI���������������ģ���ʼ���Լ����⡣

��һ���������ģ�

$n$ ��ͬѧվ��һ��ԲȦ�����е�һ��ͬѧ��������һ����ÿһ�Σ����������ͬѧ���԰��򴫸��Լ����ҵ�����ͬѧ�е�һ�����������⣩����ô�ж����ֲ�ͬ�Ĵ��򷽷�����ʹ�ô� lgd ���￪ʼ�����򣬴��� $m$ ���Ժ��ֻص� lgd �Լ������أ����ִ��򷽷���������ͬ�ķ��������ҽ��������ַ����У��ӵ����ͬѧ������˳����ɵ������ǲ�ͬ�ġ�

����˵�����֮��ϣ���������������Բ��⵽ lgd �ı��ӡ����� lgd �Ƚ��ʴȣ���������ֻ��������ȡģ $720000054000001$ �������ͺ��ˡ�

## �����ʽ
�����ж������ݡ�

����ÿ�����ݣ�һ������������ $n,m$���������⡣

## �����ʽ
����ÿ�����ݣ�һ��һ����Ȼ����ʾ�𰸡�

```input1
5 7
5 5
5 4
5 5
5 9
```

```output1
14
2
6
2
72
```

```input2
100000 998684
100000 998671
100000 998110
```

```output2
513030267786335
0
570065615362699
```

## ��ʾ
**�������������ԡ�**

**�����ж������ݡ�**

**��ע�ⳣ�����Ӵ����ĳ���Ч�ʼ��ռ�ռ���ϵ�Ӱ�졣**

���ݷ�Χ���±���ʾ��

|���ݵ���|$n$|$m$|��������|��ֵ|��������|��������|
|----|----|----|----|----|----|----|
|$1\sim6$|$=100$|$\le100$|$\le5$|$5$|A|0|
|$7\sim12$|$=10^5$|$\le10^6$|$\le5$|$15$|A|1|
|$13\sim18$|$=10^6$|$\le2\times10^6$|$\le5$|$10$|A|2|
|$19\sim24$|$=2\times10^5$|$\le10^{1000}$|$\le5$|$20$|A|3|
|$25\sim30$|$\le6\times10^6$|$\le10^{30}$|$\le50$|$20$||4|
|$31\sim36$|$\le6\times10^6$|$\le10^{10^4}$|$\le2500$|$30$||5|

�������� A����������� $n$ ȫ����ͬ��

���� $100\%$ �����ݣ�$n\in\{10,13,100,10^3,10^4,10^5,2\times10^5,6\times10^5,10^6,6\times10^6\}$��

---

lgd �����⽻�����ʱ��ͬʱ����������һ�δ��룬������ʲô�þͲ�֪���ˡ�

```cpp
typedef long long i64;
typedef unsigned long long u64;
typedef __uint128_t u128;
struct Mod64 {
  Mod64() : n(0) {}
  Mod64(u64 n) : n(init(n)) {}
  static u64 modulus() { return mod; }
  static u64 init(u64 w) { return reduce(u128(w) * r2); }
  static void setmod(u64 m) {
    mod = m;
    inv = 1;
    for (int i = 0; i < 6; ++i) inv *= 2 + inv * m;
    r2 = -u128(m) % m;
  }
  static u64 reduce(u128 x) {
    u64 y = (x + u128(u64(x) * inv) * mod) >> 64;
    return i64(y) > mod ? y - mod : y;
  }
  Mod64& operator+=(Mod64 rhs) {
    n += rhs.n - mod;
    if (i64(n) < 0) n += mod;
    return *this;
  }
  Mod64& operator-=(Mod64 rhs) {
    if (n < rhs.n)
      n += mod - rhs.n;
    else
      n -= rhs.n;
    return *this;
  }
  Mod64 operator-() const {
    if (!n) return *this;
    Mod64 rhs;
    rhs.n = mod - n;
    return rhs;
  }
  Mod64 operator+(Mod64 rhs) const { return Mod64(*this) += rhs; }
  Mod64 operator-(Mod64 rhs) const { return Mod64(*this) -= rhs; }
  Mod64& operator*=(Mod64 rhs) {
    n = reduce(u128(n) * rhs.n);
    return *this;
  }
  Mod64 operator*(Mod64 rhs) const { return Mod64(*this) *= rhs; }
  u64 get() const { return reduce(n); }
  static u64 mod, inv, r2;
  u64 n;
};
u64 Mod64::mod, Mod64::inv, Mod64::r2;
```

