## ��Ŀ����
Cows are such finicky eaters. Each cow has a preference for certain foods and drinks, and she will consume no others.

Farmer John has cooked fabulous meals for his cows, but he forgot to check his menu against their preferences. Although he might not be able to stuff everybody, he wants to give a complete meal of both food and drink to as many cows as possible.

Farmer John has cooked F (1 �� F �� 100) types of foods and prepared D (1 �� D �� 100) types of drinks. Each of his N (1 �� N �� 100) cows has decided whether she is willing to eat a particular food or drink a particular drink. Farmer John must assign a food type and a drink type to each cow to maximize the number of cows who get both.

Each dish or drink can only be consumed by one cow (i.e., once food type 2 is assigned to a cow, no other cow can be assigned food type 2).


## �����ʽ
Line 1: Three space-separated integers: N, F, and D


Lines 2..N+1: Each line i starts with a two integers Fi and Di, the number of dishes that cow i likes and the number of drinks that cow i likes. The next Fi integers  denote the dishes that cow i will eat, and the Di integers following that denote the drinks that cow i will drink.


## �����ʽ
Line 1: A single integer that is the maximum number of cows that can be fed both food and drink that conform to their wishes


## ��Ŀ����
�� $F$ ��ʳ��� $D$ �����ϣ�ÿ��ʳ�������ֻ�ܹ�һͷţ���ã���ÿͷţֻ����һ��ʳ���һ�����ϡ������� $n$ ͷţ��ÿͷţ�����Լ�ϲ����ʳ�������б�����������б��������ʹ��ͷţͬʱ���õ��Լ�ϲ����ʳ������ϡ�

����ȫ�����ݣ�$1 \le f \le 100$��$1 \le d \le 100$��$1 \le n \le 100$��

```input1
4 3 3
2 2 1 2 3 1
2 2 2 3 1 2
2 2 1 3 1 2
2 1 1 3 3
```

```output1
3
```

## ��ʾ
One way to satisfy three cows is:


Cow 1: no meal


Cow 2: Food #2, Drink #2


Cow 3: Food #1, Drink #1


Cow 4: Food #3, Drink #3


The pigeon-hole principle tells us we can do no better since there are only three kinds of food or drink. Other test data sets are more challenging, of course.


