## ��Ŀ����
���Ⲣû��ʲô��Ȥ����Ŀ������ף����졣

## ��Ŀ����
С A ��һ��**���� `A`��`P`��`C` ����**���ַ��� $S$��

С A ��Ҫ**�����ܵ�**����������ַ������������� `APC` ������**������**��ֱ���޷�������

���С A ��Ҫ�����������ַ���������ַ������Ա������ɿմ�������� `Perfect`��

Ȼ��С A ��������⣬�����������æ��

## �����ʽ
��һ��һ���� $T$ ��ʾ����������

������ $T$ ��ÿ��һ���ַ��� $S$.

## �����ʽ
**����ʹ�� Special Judge��**

�������̵Ĵ��ַ�����������һ��ɾ���ķ�����

����ÿ�����ݣ���һ�����һ����̵Ĵ��ַ�����������ܵ���̴��ַ�����������̴��ַ����ķ����ж��֣����������һ����

������һ�����һ������ $q$����ʾ���ɾ��������

������ $q$ ��ÿ�������������ֱ��ʾ����һ�β�����ɾ�����ַ� `A`��`P`��`C` **��ԭ�ַ�����**��λ�ã�**�±�� $1$ ��ʼ**��

```input1
5
PAAAAPPPCA
CAPPCPCAPAPA
PPAAAACCAAAAAAAAC
CAPPCAAPA
APPAACPPAPPPAPAAAA
```

```output1
PAAAPPA
1
5 6 9
CPPCAPAPA
1
2 4 5
PPAAAACCAAAAAAAAC
0
CPAAPA
1
2 3 5
PAAPPAPPPAPAAAA
1
1 2 6
```

```input2
1
APC

```

```output2
Perfect
1
1 2 3
```

```input3
10
PPCPAPAAACPAPACPPCPC
APPAPPAPPCPAPPCCCPPA
APPCCPPAPPAACCPPPPPP
PACPPCAPCPPCPPPAAAAC
PPPCPPCCPACAAACCCCAC
ACAAPCPAPAAAAPPACPPC
ACACPPCCPPAACPAAAAAC
APPCPCCCAPCACPAACACC
AACPCAPACPPPCAAPCCPC
PPACPPPCCAPAAAPCPAPA

```

```output3
PPCPAAPP
4
5 6 10
7 11 15
8 13 18
9 16 20
PPPPPPPA
4
1 2 10
4 5 15
7 8 16
12 13 17
PCPPPAACPPPPPP
2
1 2 4
8 9 13
PCPPPCPPPAAAAC
2
2 4 6
7 8 9
PPPCPPCCPACAAACCCCAC
0
CAAAAAPPAPP
3
1 5 6
3 7 17
4 9 20
CCPPACAAAAA
3
1 5 7
3 6 8
11 14 20
PPCCCCAAACC
3
1 2 4
9 10 11
12 14 17
CP
6
1 4 5
2 7 9
6 10 13
8 11 17
14 16 18
15 19 20
PPCPPCAAAPPAPA
2
3 5 8
10 11 16

```

## ��ʾ
**�������� #1��**  
���ڵ�һ�����ݣ��ַ���Ϊ `PAAAAPPPCA`���±�Ϊ $\{5,6,9\}$ ���ַ�����ɾ�������յõ� `PAAAPPA`��

���ڵڶ������ݣ��ַ���Ϊ `CAPPCPCAPAPA`���±�Ϊ $\{2,4,5\}$ ���ַ����������õ� `CPPCAPAPA`��

**�������� #2��**  
Ψһ��һ�������У��ַ���Ϊ `APC`����Ȼ�ܱ�ȫ������������Ҳ��Ȼ��

$1\leq T\leq 10$��$1\leq \sum |S|\leq 3\times 10^6$��

