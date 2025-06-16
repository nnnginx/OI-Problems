## ��Ŀ����
[English statement](https://www.luogu.com.cn/problem/U500140). **You must submit your code at the Chinese version of the statement.**

����ո����ǹ���أ����Ʊ�����Ȼ��������ϡ�

�����ڿɼ��ⷶΧ���������壬�����ڵ�ˮ���������˵ݽ������ɡ�

����ɫģ����ӡ���ܱ�����ҴҴ����������������ļ��������Ǹ��Ӽ������¡�

�����������������

## ��Ŀ����
С C �� $m$ ���������� $a_1\dots a_m$��ÿ�����еĳ��ȶ�Ϊ $n$��

С C ��Ҫ���Լ������а���������С��������С C �� $q$ �β�����ÿ�β�����

- Ҫô��С C ���� $x, y\ (x \neq y)$������� $a_x, a_y$ ƴ����һ���γɳ���Ϊ $2n$ ������ $b$���� $b$ ���������ȡ $b_1\dots b_n$ ��Ϊ�µ� $a_x$��$b_{n+1}\dots b_{2n}$ ��Ϊ�µ� $a_y$��
- Ҫô��С C ���� $i, j$��ϸ�ĵ�С C ��Ҫѯ���㣬����ǰ������ɴβ�����$a_{i,j}$ ��ֵ������Ҫ׼ȷ�ش��������⡣

## �����ʽ
��һ�У��������� $n, m, q$��

������ $m$ �У�ÿ�� $n$ ���������� $i$ �� $j$ ��������ʾ $a_{i,j}$��

������ $q$ �У�ÿ����������������һ�β�����ѯ�ʡ����ʽΪ��������֮һ��

- $\verb!1 x y!$ ��ʾ�� $a_x, a_y$ ������������ $1 \leq x \neq y \leq m$��
- $\verb!2 i j!$ ��ʾ��ѯ $a_{i,j}$������ $1 \leq i \leq m$��$1 \leq j \leq n$��

## �����ʽ
����ÿ��ѯ�ʣ�һ��һ����������ʾ�𰸡�

```input1
5 3 6
1 3 2 5 6
2 7 8 2 2
3 5 3 4 8
2 1 5
1 1 2
2 2 4
1 1 3
1 2 1
2 2 3
```

```output1
6
7
2

```

```input2
6 5 20
5 14 13 1 15 17
7 7 19 3 8 6
16 13 13 6 14 2
12 5 4 17 12 3
19 19 4 6 3 3
2 5 3
1 4 3
2 1 1
1 2 5
2 4 6
2 2 2
1 4 2
1 2 4
2 1 1
2 3 3
2 3 3
1 4 2
1 4 1
2 3 5
1 3 4
1 4 1
1 1 4
1 5 1
2 2 4
2 4 2

```

```output2
4
5
12
3
5
13
13
16
6
14

```

## ��ʾ
### ���ݹ�ģ��Լ��

**�������������Ժ�����������**��

��Ϊ������� Subtask �ļ����������ݴ�С�ֱ�ﵽ 18MB��50MB ���ϣ�C++ ѡ�ֿ���ѡ��ʹ������� **�����������ģ��**��

```cpp
namespace FastIO {
	char buf[1 << 21], *p1 = buf, *p2 = buf;
#define getchar() (p1 == p2 && (p1 = buf, p2 = (p1 + fread(buf, 1, 1 << 21, stdin))) == p1 ? EOF : *p1++)
	template <typename T> inline T read() { T x = 0, w = 0; char ch = getchar(); while (ch < '0' || ch > '9') w |= (ch == '-'), ch = getchar(); while ('0' <= ch && ch <= '9') x = x * 10 + (ch ^ '0'), ch = getchar(); return w ? -x : x; }
	template <typename T> inline void write(T x) { if (!x) return; write<T>(x / 10), putchar((x % 10) ^ '0'); }
	template <typename T> inline void print(T x) { if (x > 0) write<T>(x); else if (x < 0) putchar('-'), write<T>(-x); else putchar('0'); }
	template <typename T> inline void print(T x, char en) { print<T>(x), putchar(en); }
}; using namespace FastIO;
#undef getchar()
```

**����֤���� C++ ���������һ���ܹ�ͨ��������֤���� C++ �����г����ʱ�ޡ�**

---

- Subtask 0��0 pts����������
- Subtask 1��9 pts����$n \leq 10^4$��$q \leq 3000$�������������� $0$��
- Subtask 2��23 pts����$q \leq 3000$�������������� $0, 1$��
- Subtask 3��20 pts����$m \leq 5$��$q \leq 4\times 10^5$�������������� $0$��
- Subtask 4��28 pts����$q \leq 4\times 10^5$�������������� $0 \sim 3$��
- Subtask 5��20 pts�������������ơ������������� $0 \sim 4$��

�����������ݣ����� $1 \leq n\cdot m \leq 2\times 10^6$��$1 \leq m \leq 20$��$1 \leq q \leq 5\times 10^6$��$1 \leq a_{i,j} \leq 10^7$�����ڲ�����ѯ�ʣ�$1 \leq x \neq y \leq m$��$1 \leq i \leq m$��$1 \leq j \leq n$��

