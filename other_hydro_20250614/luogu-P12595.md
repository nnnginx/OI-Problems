## ��Ŀ����

������һ������Ϊ $n$ ������ $a = [a_0, a_1, \dots a_{n - 1}]$����Ҫ����֧�����²������� $q$ �Σ�

- `1 x`����������ÿ���������� $x$������ $0 \leq i < n$����ִ�� $a_i := a_i + x$������ $:=$ ��ʾ��ֵ��
- `2 x`����������ÿ���������� $x$������ $0 \leq i \lt n$����ִ�� $a_i := a_i \times x$������ $:=$ ��ʾ��ֵ��
- `3 k p`������������ $i \equiv p \pmod {2^k}$ �� $i$���� $a_i$ �ĺͶ� $998,244,353$ ȡģ�Ľ�������� $(\sum_{i = 0}^{n - 1} a_i \times [i \equiv p \pmod {2^k}]) \bmod 998,244,353$������ $[]$ ��[����ɭ����](https://baike.baidu.com/item/%E8%89%BE%E4%BD%9B%E6%A3%AE%E6%8B%AC%E5%8F%B7)��

Ϊ�˱������������ֻ��Ҫ������в��� $3$ �Ľ����**��λ����**��

����������ģ�ǳ��޴���������ṩ��һ����������������������к�ѯ�ʡ�����Բο������ʽ������������ݡ�

## �����ʽ
Ϊ�˱������������ǽ��ṩ����������������

��׼���빲���У���һ�����ĸ����� $n, q, \mathrm{minK}, \mathrm{maxK}$������ $n$ �� $q$ ��ʾ���г��ȺͲ���������$\mathrm{minK}$ �� $\mathrm{maxK}$ ��ʾ���� $k$ ����С�����ֵ���������������õ���������ֵ��  

**�����ṩ�� C++��Java��Python �������Ե������������ο����룬�������˵��/��ʾ��ֱ�Ӳο���ʹ����Щ���룬�����豻�����ж�Ϊ����**��

��׼����ڶ������������� $X, Y, Z$�������������� **32 λ�޷�������**���������������������������������������

��Ӧ�ö������º�����

```cpp
typedef uint32_t ui;
ui X, Y, Z;

ui nextInt(ui &x = X, ui &y = Y, ui &z = Z) {
  x ^= y << (z & 31);
  y ^= z >> (x & 31);
  z ^= x << (y & 31);
  x ^= x >> 5; y ^= y << 17; z ^= z >> 6;
  return x;
}
```

��������ÿ�ε��� `nextInt()` �������㶼���õ�һ�� $32$ λ�޷���������

�����׼����������� $7$ �����������Ѿ��õ��� $n$ �� $q$ ��ֵ�������������´����������� $a$��

```cpp
const int lim = 998'244'353;
std::vector<int> genArr(int n) {
  std::vector<int> ret(n);
  for (int i = 0; i < n; ++i) ret[i] = nextInt() % lim;
  return ret;
}
```
����������Ҫ���� $q$ �β�������ÿ�β������������£�

- �� `op = nextInt() % 3 + 1`
- �� $op = 1$ �� $op = 2$��ȡ `x = nextInt() % lim`
- ����**����**ȡ��`k = nextInt() % (maxK - minK + 1) + minK, p = nextInt() % (1 << k)`

������������õ�ÿ�β�������Ϣ�ˡ�



## �����ʽ
���һ��һ����������ʾ���в��� $3$ �Ľ���İ�λ���͡�

```input1
5 7 0 2
1 2 3
```

```output1
89001694
```

## ��ʾ
### ��������

���������������õ������� $a = [17,17301653,16795857,17320599,754976961]$��

�õ��Ĳ��������ǣ�
```plain
2 558452929
2 832199221
1 38834385
3 0 0
3 1 1
1 818308198
2 135235876
```

### ���ݹ�ģ��Լ��
| ���Ե��� | $n \le $ | $q \le$ | ����Լ�� |
| :-: | :-: | :-: | :-: |
| $1,2$ | $10^3$ | $10^3$ | �� |
| $3$ | $10^5$ | $10^5$ | $k=0$ |
| $4$ | $10^5$ | $10^5$ | $k=1$ |
| $5$ | $10^5$ | $10^5$ | $k = 10$ |
| $6$ | $10^5$ | $10^5$ | �� |
| $7$ | $10^5$ | $4 \times 10^7$ | �� |
| $8$ | $4 \times 10^7$ | $10^5$ | �� |
| $9, 10$ | $4 \times 10^7$ |$4 \times 10^7$ | �� |

��ȫ���Ĳ������ݣ���֤ $1 \leq n, q \leq 4 \times 10^7$��$1 \leq op \leq 3$��$0 \leq k \leq \log_2 n$��$0 \leq p < 2^k$��$0 \leq a_i,x < 998,244,353$��

Ϊ�˰���������жϵ�ǰ���Ե������Լ�������Ǳ�֤�����Ϊ $i$ �Ĳ��Ե�������� $n$ ��ĩλ����Ϊ $i \bmod 10$��

### �ο�ʵ��

��C++ �ο�ʵ�֡�
```cpp
#include <bits/stdc++.h>

typedef uint32_t ui;
int n, q, minK, maxK;
ui X, Y, Z;

ui nextInt(ui &x = X, ui &y = Y, ui &z = Z) {
  x ^= y << (z & 31);
  y ^= z >> (x & 31);
  z ^= x << (y & 31);
  x ^= x >> 5; y ^= y << 17; z ^= z >> 6;
  return x;
}

const int lim = 998'244'353;
std::vector<int> genArr(int n) {
  std::vector<int> ret(n);
  for (int i = 0; i < n; ++i) ret[i] = nextInt() % lim;
  return ret;
}

int main() {
  std::cin >> n >> q >> minK >> maxK;
  std::cin >> X >> Y >> Z;
  std::vector<int> a = genArr(n);
  for (int _ = 1; _ <= q; ++_) {
    int op = nextInt() % 3 + 1;
    if (op == 1) {
      int x = nextInt() % lim;
      //fill your code here
    } else if (op == 2) {
      int x = nextInt() % lim;
      //fill your code here
    } else {
      int k = nextInt() % (maxK - minK + 1) + minK;
      int p = nextInt() % (1 << k);
      //fill your code here
    }
  }
  //fill your code here
}
```

��Java �ο�ʵ�֡�
```java
import java.util.Scanner;

public class Main {
  private static final int lim = 998244353;
  private static long X, Y, Z;

  private static long maskToU32(long x) {
    return x & 0xFFFFFFFFL;
  }

  private static long nextInt() {
    long x = X;
    long y = Y;
    long z = Z;

    x ^= y << (z & 31);
    x = maskToU32(x);
    y ^= z >>> (x & 31);
    y = maskToU32(y);
    z ^= x << (y & 31);
    z = maskToU32(z);

    x ^= x >>> 5;
    x = maskToU32(x);
    y ^= y << 17;
    y = maskToU32(y);
    z ^= z >>> 6;
    z = maskToU32(z);

    X = x;
    Y = y;
    Z = z;

    return X;
  }

  private static int[] genArr(int n) {
    int[] ret = new int[n];
    for (int i = 0; i < n; ++i) {
      ret[i] = (int)(nextInt() % lim);
    }
    return ret;
  }

  public static void main(String[] args) {
    Scanner scanner = new Scanner(System.in);
    int n = scanner.nextInt();
    int q = scanner.nextInt();
    int minK = scanner.nextInt();
    int maxK = scanner.nextInt();
    X = scanner.nextLong();
    Y = scanner.nextLong();
    Z = scanner.nextLong();

    int[] a = genArr(n);

    for (int qId = 1; qId <= q; qId++) {
      long op = nextInt() % 3 + 1;
      if (op == 1) {
        int x = (int)(nextInt() % lim);
        // fill your code here
      } else if (op == 2) {
        int x = (int)(nextInt() % lim);
        // fill your code here
      } else {
        int k = (int)(nextInt() % (maxK - minK + 1) + minK);
        int p = (int)(nextInt() % (1 << k));
        // fill your code here
      }
    }
    // fill your code here
  }
}
```
��Python �ο�ʵ�֡�
```py
X = 0
Y = 0
Z = 0

lim = 998244353


def nextInt():
  global X, Y, Z
  x = X
  y = Y
  z = Z

  x ^= (y << (z & 31)) & 0xFFFFFFFF
  x &= 0xFFFFFFFF

  y ^= (z >> (x & 31)) & 0xFFFFFFFF
  y &= 0xFFFFFFFF

  z ^= (x << (y & 31)) & 0xFFFFFFFF
  z &= 0xFFFFFFFF

  x ^= (x >> 5)
  x &= 0xFFFFFFFF

  y ^= (y << 17) & 0xFFFFFFFF
  y &= 0xFFFFFFFF

  z ^= (z >> 6)
  z &= 0xFFFFFFFF

  X, Y, Z = x, y, z
  return X


n, q, minK, maxK = map(int, input().split())
X, Y, Z = map(int, input().split())

a = [nextInt() % lim for _ in range(n)]

for _ in range(q):
  op = nextInt() % 3 + 1
  if op == 1:
    x = nextInt() % lim
    #fill your code here
  elif op == 2:
    x = nextInt() % lim
    #fill your code here
  elif op == 3:
    k = nextInt() % (maxK - minK + 1) + minK
    p = nextInt() % (1 << k)
    #fill your code here

#fill your code here
```

