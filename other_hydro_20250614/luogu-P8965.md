## ��Ŀ����
������Ū���䣬��ν���ˣ�����������������һ�����Ӷ��ѡ�

����Ȳ����ĺ������վ�����һ�����ε��Σ�һ�����ٴ�������

����������ľżһ����һ�εı���ס����, �԰������壬������ʱ��Ļ����

������ִ��󣬶���һ����Ť���ġ�������
 
 ������ŵ��û�г��֣���ҹ���ߣ�������ֻ���������ŵģ����㰮��һ���˼�

��������ֻף���������߲������󡣡�

û�й���������Ϊ��������һ���ˣ��������������á�
 

## ��Ŀ����
����һ�� $n$ �������޸�����ÿ�����зǸ�������Ȩ������� $1 \sim n$ ��š�

����ÿһ����� $(x, y)$������ $(x, y)$ �ľ��� $\operatorname{dis}(x, y)$ Ϊ $x,y$ ����֮��Ψһ��·���ϱ�Ȩ�����͡�

����������� $x, y$������� $i$ �ļ�ֵ $\operatorname{val}_{x, y}(i)$ Ϊ $(x, i)$ �� $(y, i)$ �ľ�������ͣ���

$$ \operatorname{val}_{x, y}(i) = \operatorname{dis}(x, i) \oplus \operatorname{dis}(y, i) \textsf{��} $$

������ $q$ ��ѯ�ʣ�ÿ��ѯ�ʸ����ĸ����� $x, y, l, r$���� $\displaystyle \bigoplus_{i = l}^{r} \operatorname{val}_{x, y}(i)$ ��ֵ������

$$ \operatorname{val}_{x, y}(l) \oplus \operatorname{val}_{x, y}(l + 1) \oplus \cdots \oplus \operatorname{val}_{x, y}(r - 1) \oplus \operatorname{val}_{x, y}(r) \textsf{��} $$

������ʽ�У�$\oplus$ ��ʾ�����ư�λ���

## �����ʽ
��һ�У��������� $n, q$��

������ $n - 1$ �У�ÿ���������� $u, v, w$����ʾ $u, v$ ֮����һ��ȨֵΪ $w$ �ıߡ�

������ $q$ �У�ÿ���ĸ����� $x,y,l,r$����ʾһ��ѯ�ʡ�

## �����ʽ
��� $q$ �У�ÿ��һ��������Ϊÿ��ѯ�ʵĴ𰸡�

```input1
3 2
1 2 1
2 3 1
1 2 1 3
2 3 2 3

```

```output1
1
0

```

## ��ʾ
**���������͡�**

![](https://cdn.luogu.com.cn/upload/image_hosting/oew00pa7.png)

���������������ͼ��ʾ�����ڵ�Եľ��룬��

- $\operatorname{dis}(1, 1) = \operatorname{dis}(1, 3) = \operatorname{dis}(2, 2) = \operatorname{dis}(3, 1) = \operatorname{dis}(3, 3) = 0$ �Լ�
- $\operatorname{dis}(1, 2) = \operatorname{dis}(2, 1) = \operatorname{dis}(2, 3) = \operatorname{dis}(3, 2) = 1$��

�� $1$ �ʣ�$\operatorname{val}_{1, 2}(1) \oplus \operatorname{val}_{1, 2}(2) \oplus \operatorname{val}_{1, 2}(3) = (0 \oplus 1) \oplus (1 \oplus 0) \oplus (0 \oplus 1) = 1 \oplus 1 \oplus 1 = 1$��

�� $2$ �ʣ�$\operatorname{val}_{2, 3}(2) \oplus \operatorname{val}_{2, 3}(3) = (0 \oplus 1) \oplus (1 \oplus 0) = 1 \oplus 1 = 0$��

---

**�����ݷ�Χ��**

**�������������ԡ�**

| �������� | $n \le$ | $q \le$ | ��ֵ |
| :----------: | :----------: | :----------: | :----------: |
| 1 | $100$ | $10$ | 24 |
| 2 | $10^6$ | $10$ | 14 |
| 3 | $100$ | $10^6$ | 14 |
| 4 | $10^6$ | $10^6$ | 48 |

���� $100\%$ �����ݣ���֤ $1 \le n, q \le {10}^6$��$1 \le u, v, x, y \le n$��$1 \le l \le r \le n$��$0 \le w < 2^{31}$��

---

**����ʾ��**

������� I/O ���ﵽ 60 MiB����ע�� I/O Ч�ʡ�

