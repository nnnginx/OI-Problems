## ��Ŀ����
You're the boss of a building company. At the beginning, there are $g$ types of employees in the company, and different types of employees have different occupations. For the $i$-th type of employees, their occupation can be numbered as $t_i$ and there are $u_i$ employees in total.

There are $n$ building projects in the market waiting to be undertaken. To undertake the $i$-th project, your company must meet $m_i$ requirements. The $j$-th requirement requires that your company has at least $b_{i, j}$ employees whose occupation is $a_{i, j}$. After undertaking the project, your company will become more famous and will attract $k_i$ types of employees to join your company. The occupation of the $j$-th type of employees is $c_{i, j}$ and there are $d_{i, j}$ employees in total.

You can undertake any number of projects in any order. Each project can be undertaken at most once. Calculate the maximum number of projects you can undertake.

Note that employees are not consumables. After undertaking a project the number of employees in your company won't decrease.

## �����ʽ
There is only one test case in each test file.

The first line of the input first contains an integer $g$ ($1 \le g \le 10^5$) indicating the number of types of employees in the company at the beginning. Then $g$ pairs of integers $t_1, u_1, t_2, u_2, \cdots t_g, u_g$ follow ($1 \le t_i, u_i \le 10^9$), where $t_i$ and $u_i$ indicate that there are $u_i$ employees whose occupation is $t_i$. It's guaranteed that for all $1 \le i < j \le g$ we have $t_i \ne t_j$.

The second line contains an integer $n$ ($1 \le n \le 10^5$) indicating the number of projects waiting to be undertaken.

For the following $2n$ lines, each two lines describe a project.

The $(2i - 1)$-th line first contains an integer $m_i$ ($0 \le m_i \le 10^5$) indicating the number of requirements to undertake the $i$-th project. Then $m_i$ pairs of integers $a_{i, 1}, b_{i, 1}, a_{i, 2}, b_{i, 2}, \cdots, a_{i, m_i}, b_{i, m_i}$ follow ($1 \le a_{i, j}, b_{i, j} \le 10^9$) where $a_{i, j}$ and $b_{i, j}$ indicate that the company is required to have at least $b_{i, j}$ employees whose occupation is $a_{i, j}$. It's guaranteed that for all $1 \le x < y \le m_i$ we have $a_{i, x} \ne a_{i, y}$.

The $2i$-th line first contains an integer $k_i$ ($0 \le k_i \le 10^5$) indicating the number of types of employees to join the company after undertaking the $i$-th project. Then $k_i$ pairs of integers $c_{i, 1}, d_{i, 1}, c_{i, 2}, d_{i, 2}, \cdots, c_{i, k_i}, d_{i, k_i}$ follow ($1 \le c_{i, j}, d_{i, j} \le 10^9$) where $c_{i, j}$ and $d_{i, j}$ indicate that there are $d_{i, j}$ employees whose occupation is $c_{i, j}$ joining the company. It's guaranteed that for all $1 \le x < y \le k_i$ we have $c_{i, x} \ne c_{i, y}$.

It's guaranteed that neither the sum of $m_i$ nor the sum of $k_i$ will exceed $10^5$.

## �����ʽ
Output one line containing one integer indicating the maximum number of projects you can undertake.

## ��Ŀ����
**����Ŀ������**

����һ�ҽ�����˾���ϰ塣һ��ʼ����˾���� $g$ ��Ա����ÿһ��Ա��������һ�����֡��� $i$ ��Ա���Ĺ��ֱ��Ϊ $t_i$������ $u_i$ �ˡ�

�г��Ϲ��� $n$ ��̵ȴ��нӡ���Ҫ�нӵ� $i$ ��̣����Ĺ�˾��Ҫ���� $m_i$ ��Ҫ�����е� $j$ ��Ҫ�����Ĺ�˾�����й��ֱ��Ϊ $a_{i, j}$ ��Ա�� $b_{i, j}$ �ˡ��нӸù��̺����Ĺ�˾������������������� $k_i$ ��Ա�����빫˾�����е� $j$ ��Ա���Ĺ��ֱ��Ϊ $c_{i, j}$������ $d_{i, j}$ �ˡ�

�����԰�����˳��н����������Ĺ��̣�ÿ������ֻ�ܱ��н�һ�Ρ�������ܳнӶ��ٹ��̡�

��ע�⣺Ա����������Ʒ���н�һ��̺�Ա��������������١�

**�������ʽ��**

ÿ�������ļ�����һ��������ݡ�

��һ����������һ������ $g$��$1 \le g \le 10^5$����ʾһ��ʼ��˾��Ա���������������������� $g$ ������ $t_1, u_1, t_2, u_2, \cdots t_g, u_g$��$1 \le t_i, u_i \le 10^9$�������� $t_i$ �� $u_i$ ��ʾһ��ʼ���ֱ��Ϊ $t_i$ ��Ա������ $u_i$ �ˡ���֤�������� $1 \le i < j \le g$ �� $t_i \ne t_j$��

�ڶ�������һ������ $n$��$1 \le n \le 10^5$����ʾ�ȴ��нӵĹ���������

���ڽ����� $2n$ �У�ÿ��������һ��̡�

�� $(2i - 1)$ ����������һ������ $m_i$��$0 \le m_i \le 10^5$����ʾ�нӵ� $i$ ����м���Ҫ�󡣽��������� $m_i$ ������ $a_{i, 1}, b_{i, 1}, a_{i, 2}, b_{i, 2}, \cdots, a_{i, m_i}, b_{i, m_i}$��$1 \le a_{i, j}, b_{i, j} \le 10^9$�������� $a_{i, j}$ �� $b_{i, j}$ ��ʾ��˾����Ҫ�й��ֱ��Ϊ $a_{i, j}$ ��Ա�� $b_{i, j}$ �ˡ���֤�������� $1 \le x < y \le m_i$ �� $a_{i, x} \ne a_{i, y}$��

�� $2i$ ����������һ������ $k_i$��$0 \le k_i \le 10^5$����ʾ�нӵ� $i$ ���֮���м���Ա�����빫˾������������ $k_i$ ������  $c_{i, 1}, d_{i, 1}, c_{i, 2}, d_{i, 2}, \cdots, c_{i, k_i}, d_{i, k_i}$��$1 \le c_{i, j}, d_{i, j} \le 10^9$�������� $c_{i, j}$ �� $d_{i, j}$ ��ʾ���ֱ��Ϊ $c_{i, j}$ ��Ա���� $d_{i, j}$ �˼��빫˾����֤�������� $1 \le x < y \le k_i$ �� $c_{i, x} \ne c_{i, y}$��

��֤ $m_i$ �� $k_i$ ֮�;������� $10^5$��

**�������ʽ��**

���һ��һ��������ʾ����ܳнӼ���̡�

**���������͡�**

�����������£��� $(t, u)$ ��ʾ����Ϊ $t$ ��Ա���� $u$ ����

���ȳн�û���κ�Ҫ��ĵ� $5$ ��̣��нӺ���Ϊ $3$ �� $2$ ��Ա�����빫˾����˾������Ա��Ϊ $\{(1, 2), (2, 1), (3, 2)\}$��

�������нӵ� $1$ ��̣��нӺ�û��Ա�����빫˾����˾������Ա����Ϊ $\{(1, 2), (2, 1), (3, 2)\}$��

�������нӵ� $2$ ��̣��нӺ���Ϊ $3$ �� $2$ ��Ա�����Լ�����Ϊ $2$ �� $1$ ��Ա�����빫˾����˾������Ա��Ϊ $\{(1, 2), (2, 2), (3, 4)\}$��

�������нӵ� $4$ ��̣��нӺ���Ϊ $1$ �� $3$ ��Ա�����빫˾����˾������Ա��Ϊ $\{(1, 5), (2, 2), (3, 4)\}$��

���ڹ���Ϊ $2$ ��Ա������ $3$ ��������޷��нӽ�ʣ�ĵ� $3$ ��̡�

```input1
2 2 1 1 2
5
1 3 1
0
2 1 1 2 1
2 3 2 2 1
3 1 5 2 3 3 4
1 2 5
3 2 1 1 1 3 4
1 1 3
0
1 3 2
```

```output1
4
```

## ��ʾ
We explain the sample test case as follows. Let $(t, u)$ indicate $u$ employees whose occupation is $t$.

First, undertake the $5$-th project with no requirements. After undertaking the project, there are $2$ employees, whose occupation is $3$, joining the company. The company now have these employees: $\{(1, 2), (2, 1), (3, 2)\}$.

Next, undertake the $1$-st project. After undertaking the project, no employee joins the company. The company now still have these employees: $\{(1, 2), (2, 1), (3, 2)\}$.

Next, undertake the $2$-nd project. After undertaking the project, there are $2$ employees, whose occupation is $3$, and $1$ employee, whose occupation is $2$, joining the company. The company now have these employees: $\{(1, 2), (2, 2), (3, 4)\}$.

Next, undertake the $4$-th project. After undertaking the project, there are $3$ employees, whose occupation is $1$, joining the company. The company now have these employees: $\{(1, 5), (2, 2), (3, 4)\}$.

As the company does not have $3$ employees whose occupation is $2$, we cannot undertake the $3$-rd project.

