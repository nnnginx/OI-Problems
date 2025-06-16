## ��Ŀ����
Just like humans, cows often appreciate feeling they are unique in some way. Since Farmer John's cows all come from the same breed and look quite similar, they want to measure uniqueness in their names.

Each cow's name has some number of substrings. For example, "amy" has substrings {a, m, y, am, my, amy}, and "tommy" would have the following substrings: {t, o, m, y, to, om, mm, my, tom, omm, mmy, tomm, ommy, tommy}.

A cow name has a "uniqueness factor" which is the number of substrings of that name not shared with any other cow. For example, If amy was in a herd by herself, her uniqueness factor would be 6. If tommy was in a herd by himself, his uniqueness factor would be 14. If they were in a herd together, however, amy's uniqueness factor would be 3 and tommy's would be 11.

Given a herd of cows, please determine each cow's uniqueness factor.

## �����ʽ
The first line of input will contain $N$ ($1 \le N \le 10^5$). The following $N$ lines will each contain the name of a cow in the herd. Each name will contain only lowercase characters a-z. The total length of all names will not exceed $10^5$.


## �����ʽ
Output $N$ numbers, one per line, describing the uniqueness factor of each cow.


## ��Ŀ����
### ��Ŀ����

��������һ������ţҲ����ϣ����ĳЩ����е��Լ����ڲ�ͬ������ Farmer John ����ţ������ͬһƷ������۷ǳ����ƣ�����ϣ��ͨ�����������������ԡ�

ÿͷ��ţ�����ֶ���һЩ���ַ��������磬"amy" �����ַ���Ϊ {a, m, y, am, my, amy}���� "tommy" �����ַ���Ϊ {t, o, m, y, to, om, mm, my, tom, omm, mmy, tomm, ommy, tommy}��

һͷ��ţ��������һ�������������ӡ������������в����κ�������ţ��������ַ��������������磬��� amy ������һ��ţȺ�У����Ķ���������Ϊ 6����� tommy ������һ��ţȺ�У����Ķ���������Ϊ 14��Ȼ�������������һ��ţȺ�У�amy �Ķ���������Ϊ 3���� tommy �Ķ���������Ϊ 11��

����һ��ţȺ�������ÿͷ��ţ�Ķ��������ӡ�

### �����ʽ

����ĵ�һ�а��� $N$��$1 \le N \le 10^5$������������ $N$ ��ÿ�а���ţȺ��һͷ��ţ�����֡�ÿ�����ֽ�����Сд��ĸ a-z���������ֵ��ܳ��Ȳ����� $10^5$��

### �����ʽ

��� $N$ �����֣�ÿ��һ������ʾÿͷ��ţ�Ķ��������ӡ�

```input1
3
amy
tommy
bessie
```

```output1
3
11
19
```

