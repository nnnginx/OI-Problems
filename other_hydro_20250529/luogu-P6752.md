## ��Ŀ����
����һ�� **Grader ������**��

����ʱ�� 10s�����޳������������ڴ�� 16MB��

���������� $190$���������ѡ��ķ����ɵ� $100$ �֡�

#### ����ע������
- ��Ĵ����в�Ӧ���� `cmp.h`����Ӧ���ڿ�ͷ������������������������
   - `void bit_set(int);`
   - `int bit_get(int);`
- ��Ĵ�����Ӧ��ʵ���������� ��
   - `void remember(int a);`
   - `int compare(int b);`

���仰˵�������������µĴ���ģ���б�д����
```cpp
#include <bits/stdc++.h>
using namespace std;
do something...
extern "C" void bit_set(int);
extern "C" int bit_get(int);
extern "C" void remember(int a) {
    do something...
}
extern "C" int compare(int b) {
    do something...
}
```

## ��Ŀ����
������һ����һά����Ϊ $4096$���ڶ�ά����Ϊ $10240$ �Ķ�ά $01$ ���� $mem$����ʼʱ����ֵΪ $0$��

����Ҫ��д�� $01$ ������ִ�е��������� `void remember(int a)` �� `int compare(int b)`��

#### ʵ��ϸ��

`void remember(int a)` ��

- ��֤ $0\le a\le 4095$��
- �����Ե��� `void bit_set(int ad)`����������Ҫ��֤ $1\le ad \le 10240$��
  - ��ᵼ�� $mem_{a,ad}=1$��

`int compare(int b)`��

- ��֤ $0\le b\le 4095$��
- ����Ҫ�� $a$ ��  $b$ ���бȽϣ����� $a$ δ֪��
  -  �� $b<a$���뷵�� $-1$��
  - �� $b=a$���뷵�� $0$��
  - �� $b>a$���뷵�� $1$��
- �����Ե��� `int bit_get(int ad)`����������Ҫ��֤ $1\le ad \le 10240$��
  - ��᷵�� $mem_{a,ad}$ ��ֵ

#### ����

��Ӧ��ʵ�������������� `void remember(int a)` �� `int compare(int b)` �����̶��ϼ��� `void bit_set(int ad)` �� `int bit_get(int ad)` �ĵ��ô�����

���ĵ÷�������α������㣺

```
define AllMemory = array [0..4095][1..10240] of bits
set AllMemory to zeros
for a = 0..4095:
    define bit_set(address): AllMemory[a][address] = 1
    remember(a)
let maxA= the maximum number of bit_set() calls executed for any a
for (a,b) �� {0..4095}��{0..4095} in random order (i.e. all valid pairs (a,b) are considered, in some random order)
    define bit_get(address): return AllMemory[a][address]
    answer =compare(b)
    if answer for comparing a and b is incorrect : your score = 0; exit
let maxB = the maximum number of bit_get() calls executed for any (a,b) pair
T=maxA + maxB
If (T>20): your score = 0; exit
else your score = 1 + 9 * (21�C T); exit
```

## ��ʾ
#### ����

- ������Ľ�����������������ʵ��ϸ�ڲ��֣������䡣

- ���Ľ��������������� 10s �ڵ��� $4096$ ��  `void remember(int a)`  �� $4096\times 4096$ �� `int compare(int b)`��
#### ˵��
�������� [Balkan Olympiad in Informatics 2011](http://www.boi2011.ro/boi2011/) [Day 2](http://www.boi2011.ro/boi2011/?pagina=probleme) [T1 cmp](http://www.boi2011.ro/resurse/tasks/cmp.zip)��

��л @[tiger2005](https://www.luogu.com.cn/user/60864) �ṩ�Ľ����⡣

