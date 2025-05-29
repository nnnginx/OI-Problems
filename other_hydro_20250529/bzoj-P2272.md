## ��Ŀ����

Like all bovines��Farmer John's cows speak the peculiar ��Cow�� language��Like so many languages��each word in this language comprises a sequence of upper and lowercase letters ��$\text{A}\sim\text{Z}$ and $\text{a}\sim \text{z}$����A word is valid if and only if each ordered pair of adjacent letters in the word is a valid pair��

Farmer John��ever worried that his cows are plotting against him��recently tried to eavesdrop on their conversation��He overheard one word before the cows noticed his presence��The Cow language is spoken so quickly��and its sounds are so strange��that all that Farmer John was able to perceive was the total number of uppercase letters��$U$ and the total number of lowercase letters��$L$ in the word��

Farmer John knows all $P$ valid ordered pairs of adjacent letters��He wishes to know how many different valid words are consistent with his limited data��However��since this number may be very large��he only needs the value modulo $97654321$��

Լ������ţ�����Ǳ����������ġ�ţ���ţ��ʹ�õ���ĸ����Ӣ����ĸ���д�Сд֮�֡�ţ���д��� $P$ ���Ϸ��Ĵ��أ�ÿ�����ض���������ĸ��ɡ�ţ��ĵ���������ĸ��ɵ����У�һ��������������ĳ�Ҫ�������������ڵ���ĸ���ǺϷ��Ĵ��ء�

Լ������������ţ������ı���������������һֱ��͵�����ǵĶԻ������ǣ�ţ��̫�����ˣ���ģģ������ֻ������һ�����ʣ���ȷ��������������� $U$ ����д��ĸ��$L$ ��Сд��ĸ����������֪����������������������ģ���ô�ж����ֿ������أ������������̫���ˣ���ֻҪ�����ȡ $97654321$ �������Ϳ����ˡ�

## �����ʽ

* Line $1$��Three space-separated integers��$U,L$ and $P$

* Lines $2 \dots P + 1$��Two letters ��each of which may be uppercase or lowercase����representing one valid ordered pair of adjacent letters in Cow��

**��һ�У������ÿո������������**$U,L$ **��** $P$**��**

**�ڶ��е�** $P + 1$ **�У���** $i + l$ **��������ĸ����ʾ��** $i$ **�����أ�û��������������ȫ��ͬ�ġ�**

## �����ʽ

* Line $1$��A single integer��the number of valid words consistent with Farmer John's data mod $97654321$��

������������ʾ���������ĵ����������� $97654321$ ��������

```input1
2 2 7
AB
ab
BA
ba
Aa
Bb
bB
```

```output1
7
```

## ��������1

INPUT DETAILS��  
The word Farmer John overheard had $2$ uppercase and $2$ lowercase letters��The valid pairs of adjacent letters are $AB,ab,BA,ba,Aa,Bb$ and $bB$��

���ܵĵ���Ϊ $\text{AabB��Abba��abBA��BAab��BbBb��bBAa��bBbB}$ �� $7$ ����

## ��Ŀ��Դ

Gold

## ���ݹ�ģ��Լ��

$100\%$ ���������㣺$1 \le U,L \le 250$��$1 \le P \le 200$��
