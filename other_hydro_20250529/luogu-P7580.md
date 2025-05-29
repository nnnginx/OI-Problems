## ��Ŀ����
monsters ϲ��������������Ҫ��һ�������������⡣

## ��Ŀ����
������֪��$i$ �ı�׼�ֽ���ʽΪ��$\prod\limits_{j=1}^{k_i}p_{i,j}^{c_{i,j}}$��

����һ������ $a$������Ϊ $n$��

���� $f(x)=\sum\limits_{d|x}\left({a_{\frac{x}{d}}\times\prod\limits_{i=1}^{k_d}{C_{c_{d,i}+m}^{m}}}\right)$��������Ҫ����� $f(1),f(2),f(3),\cdots ,f(n)$������ $m$ �Ǹ���������

���� monsters ��ϲ��̫�����������Ҫ�������ģ $998244353$ ��ֵ��

���⣬Ϊ�˱����������������������ʹ��������������ݣ�����ֻ��Ҫ��������д𰸵����͡�

����㲻֪�� $C$ ��ʲô��$C_n^m=\dfrac{n!}{m!(n-m)!}$������ $!$ ����׳ˡ�

## �����ʽ
���빲��һ�С�

��һ�У������Ǹ����� $n,m,seed$��

����Ҫ�ڳ����е��� $n$ ��������������```randomdigit```�����õ� $a$��

## �����ʽ
�������һ��һ��������Ϊ���� $f(x)$ �����͡�

```input1
3 0 12345678
```

```output1
175092810
```

```input2
114514 100000 1919810
```

```output2
212218651

```

```input3
9919810 2 12121121
```

```output3
204065242
```

## ��ʾ
**����������**

C/C++:
```cpp
#define uint unsigned int
uint seed;
inline uint randomdigit(){
	seed^=seed<<13;
	seed^=seed>>17;
	seed^=seed<<5;
	return seed;
}
```
pascal:
```pascal
var seed:dword;
function randomdigit:dword;
begin
	seed:=seed xor(seed shl 13);
	seed:=seed xor(seed shr 17);
	seed:=seed xor(seed shl 5);
	randomdigit:=seed;
end;
```

python3:
```python
seed = 0 # please input seed
mod = 1 << 32
def randomdigit():
    global seed
    seed ^= (seed << 13) % mod
    seed ^= (seed >> 17) % mod
    seed ^= (seed << 5) % mod
    return seed
```

---

**��������**

���� $a$ Ϊ $506005380,3857352168,531380003$��

$f(1),f(2),f(3)$ ģ $998244353$ ��ֵ�ֱ�Ϊ $506005380,370380136,39141030$��

---

**���ݷ�Χ**

���� $100\%$ �����ݣ�$0\le m\le 10^5,1\le n\le 10^7,0\le a_1,a_2,\cdots,a_n,seed<2^{32}$��

- Subtask $1$��$30\%$ �����ݣ���$n\le 10^6,m\le 10^5$��

�ڴ� Subtask �У�

�� $10\%$ �����ݣ����� $m=0$��

���� $10\%$ �����ݣ����� $n\le 100$��
- Subtask $2$��ʣ�� $70\%$ �����ݣ���$n\le 10^7,m\le 3$��

**��ʾ**

��ע��ռ����ƺͳ������ӶԳ�������Ч�ʵ�Ӱ��

