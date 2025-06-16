## 题目描述

扶苏有一个长度为 $n$ 的数列 $a = [a_0, a_1, \dots a_{n - 1}]$。您要帮她支持如下操作，共 $q$ 次：

- `1 x`：给数列里每个数都加上 $x$，即对 $0 \leq i < n$，都执行 $a_i := a_i + x$，其中 $:=$ 表示赋值。
- `2 x`：给数列里每个数都乘上 $x$，即对 $0 \leq i \lt n$，都执行 $a_i := a_i \times x$，其中 $:=$ 表示赋值。
- `3 k p`：对所有满足 $i \equiv p \pmod {2^k}$ 的 $i$，求 $a_i$ 的和对 $998,244,353$ 取模的结果，即求 $(\sum_{i = 0}^{n - 1} a_i \times [i \equiv p \pmod {2^k}]) \bmod 998,244,353$，其中 $[]$ 是[艾佛森括号](https://baike.baidu.com/item/%E8%89%BE%E4%BD%9B%E6%A3%AE%E6%8B%AC%E5%8F%B7)。

为了避免输出过大，你只需要输出所有操作 $3$ 的结果的**按位异或和**。

本题的输入规模非常巨大，因此我们提供了一个随机数生成器来生成数列和询问。你可以参考输入格式来具体查阅内容。

## 输入格式
为了避免读入过大，我们将提供如下数据生成器：

标准输入共两行，第一行有四个整数 $n, q, \mathrm{minK}, \mathrm{maxK}$。其中 $n$ 和 $q$ 表示数列长度和操作次数，$\mathrm{minK}$ 和 $\mathrm{maxK}$ 表示输入 $k$ 的最小和最大值。数据生成器将用到这两个数值。  

**我们提供了 C++、Java、Python 三种语言的数据生成器参考代码，你可以在说明/提示中直接参考和使用这些代码，而无需被担心判定为作弊**。

标准输入第二行有三个参数 $X, Y, Z$，这三个参数是 **32 位无符号整型**，数据生成器将利用这三个参数生成随机数。

你应该定义如下函数：

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

接下来，每次调用 `nextInt()` 函数，你都将得到一个 $32$ 位无符号整数。

读入标准输入里的两行 $7$ 个整数后，你已经得到了 $n$ 和 $q$ 的值，接下来按如下代码生成数列 $a$：

```cpp
const int lim = 998'244'353;
std::vector<int> genArr(int n) {
  std::vector<int> ret(n);
  for (int i = 0; i < n; ++i) ret[i] = nextInt() % lim;
  return ret;
}
```
接下来，你要生成 $q$ 次操作，对每次操作，方法如下：

- 令 `op = nextInt() % 3 + 1`
- 若 $op = 1$ 或 $op = 2$，取 `x = nextInt() % lim`
- 否则**依次**取：`k = nextInt() % (maxK - minK + 1) + minK, p = nextInt() % (1 << k)`

这样，你就能拿到每次操作的信息了。



## 输出格式
输出一行一个整数，表示所有操作 $3$ 的结果的按位异或和。

```input1
5 7 0 2
1 2 3
```

```output1
89001694
```

## 提示
### 样例解释

调用数据生成器得到的序列 $a = [17,17301653,16795857,17320599,754976961]$；

得到的操作依次是：
```plain
2 558452929
2 832199221
1 38834385
3 0 0
3 1 1
1 818308198
2 135235876
```

### 数据规模与约定
| 测试点编号 | $n \le $ | $q \le$ | 特殊约定 |
| :-: | :-: | :-: | :-: |
| $1,2$ | $10^3$ | $10^3$ | 无 |
| $3$ | $10^5$ | $10^5$ | $k=0$ |
| $4$ | $10^5$ | $10^5$ | $k=1$ |
| $5$ | $10^5$ | $10^5$ | $k = 10$ |
| $6$ | $10^5$ | $10^5$ | 无 |
| $7$ | $10^5$ | $4 \times 10^7$ | 无 |
| $8$ | $4 \times 10^7$ | $10^5$ | 无 |
| $9, 10$ | $4 \times 10^7$ |$4 \times 10^7$ | 无 |

对全部的测试数据，保证 $1 \leq n, q \leq 4 \times 10^7$，$1 \leq op \leq 3$，$0 \leq k \leq \log_2 n$，$0 \leq p < 2^k$，$0 \leq a_i,x < 998,244,353$。

为了帮助你快速判断当前测试点的特殊约定，我们保证：编号为 $i$ 的测试点所读入的 $n$ 的末位数字为 $i \bmod 10$。

### 参考实现

【C++ 参考实现】
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

【Java 参考实现】
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
【Python 参考实现】
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

