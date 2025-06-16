## ��Ŀ����
After having drifted about in a small boat for a couple of days, Akira Crusoe Maeda was finally cast ashore on a foggy island. Though he was exhausted and despaired, he was still fortunate to remember a legend of the foggy island, which he had heard from patriarchs in his childhood. This must be the island in the legend. In the legend, two tribes have inhabited the island, one is divine and the other is devilish, once members of the divine tribe bless you, your future is bright and promising, and your soul will eventually go to Heaven, in contrast, once members of the devilish tribe curse you, your future is bleak and hopeless, and your soul will eventually fall down to Hell.

In order to prevent the worst-case scenario, Akira should distinguish the devilish from the divine. But how? They looked exactly alike and he could not distinguish one from the other solely by their appearances. He still had his last hope, however. The members of the divine tribe are truth-tellers, that is, they always tell the truth and those of the devilish tribe are liars, that is, they always tell a lie.

He asked some of them whether or not some are divine. They knew one another very much and always responded to him "faithfully" according to their individual natures (i.e., they always tell the truth or always a lie). He did not dare to ask any other forms of questions, since the legend says that a devilish member would curse a person forever when he did not like the question. He had another piece of useful informationf the legend tells the populations of both tribes. These numbers in the legend are trustworthy since everyone living on this island is immortal and none have ever been born at least these millennia.

You are a good computer programmer and so requested to help Akira by writing a program that classifies the inhabitants according to their answers to his inquiries.

## �����ʽ
The input consists of multiple data sets, each in the following format :

```
n p1 p2
xl yl a1
x2 y2 a2
...
xi yi ai
...
xn yn an
```

The first line has three non-negative integers n, p1, and p2. n is the number of questions Akira asked. pl and p2 are the populations of the divine and devilish tribes, respectively, in the legend. Each of the following n lines has two integers xi, yi and one word ai. xi and yi are the identification numbers of inhabitants, each of which is between 1 and p1 + p2, inclusive. ai is either yes, if the inhabitant xi said that the inhabitant yi was a member of the divine tribe, or no, otherwise. Note that xi and yi can be the same number since "are you a member of the divine tribe?" is a valid question. Note also that two lines may have the same x's and y's since Akira was very upset and might have asked the same question to the same one more than once.

You may assume that n is less than 1000 and that p1 and p2 are less than 300. A line with three zeros, i.e., 0 0 0, represents the end of the input. You can assume that each data set is consistent and no contradictory answers are included.

## �����ʽ
For each data set, if it includes sufficient information to classify all the inhabitants, print the identification numbers of all the divine ones in ascending order, one in a line. In addition, following the output numbers, print end in a line. Otherwise, i.e., if a given data set does not include sufficient information to identify all the divine members, print no in a line.

## ��Ŀ����
### ��Ŀ����
��С����Ư���˼����Akira Crusoe Maeda ���ڱ��׵���һ�������ɵĵ��ϡ�������ƣ���������������ѣ�������Ȼ���˵ؼǵ���ͯ��ʱ���峤��������������˵����һ���Ǵ�˵�еĵ��졣��˵�������������ס�ڵ��ϣ�һ������ʥ�ģ���һ����а��ģ�һ����ʥ����ĳ�Ա�����㣬���δ���ͻ������ϣ�������������ջ�ȥ���ã����֮�£�һ��а����ĳ�Ա�����㣬���ǵ�δ���ͻ���������������������ջ�׹�������

Ϊ�˷�ֹ������������Akira Crusoe Maeda Ӧ�����ֶ�ħ�����顣������ô�������ǿ�������ȫһ�������޷���ƾ����������ǡ�Ȼ��������������ϣ������ʥ����ĳ�Ա��˵ʵ�����ˣ�Ҳ����˵����������˵ʵ������а����ĳ�Ա����ƭ�ӣ�Ҳ���������������ѡ�

���������е�һЩ���Ƿ���Щ����ʥ�ġ����Ǳ˴˷ǳ��˽⣬���Ǹ����Լ��ĸ��ԡ���ʵ�ء���Ӧ����������������˵ʵ�������ѣ������������κ�������ʽ�����⣬��Ϊ��˵�У���һ����ħ��Ա��ϲ���������ʱ��������Զ����һ���ˡ�������һ�����õ���Ϣ����˵����������������˿ڡ���˵�е���Щ������ֵ�������ģ���Ϊ������������ϵ�ÿ���˶��ǲ���ģ��������⼸ǧ����û���˳�������

����һ������ļ��������Ա����˱�Ҫ����� Akira ��дһ�����򣬸��ݾ��������ѯ�ʵĻش�����ǽ��з��ࡣ
### �����ʽ
�����ɶ�����ɣ�ÿ�����Ե�ĸ�ʽ���£�
```
n p1 p2
xl yl a1
x2 y2 a2
...
xi yi ai
...
xn yn an
```
��һ���������Ǹ����� $n$��$p_1$ �� $p_2$��$n$ �� Akira ���������������$p_l$ �� $p_2$ �ֱ��Ǵ�˵����ʥ����Ͷ�ħ������˿ڡ��������� $n$ ���е�ÿһ�ж����������� $x_i$��$y_i$ ��һ������ $a_i$��$x_i$ �� $y_i$ �Ǿ����ʶ��ţ�ÿ��ʶ����� $1$ �� $p_1+p_2$������ $1$ �� $p_1+p_2$ ��֮�䡣$a_i$ Ҫô�ǿ϶��ģ�Ҫô�Ƿ񶨵ġ���ע�⣬$x_i$ �� $y_i$ ������ͬһ�����֣���Ϊ����������ĳ�Ա�𣿡���һ����Ч�����⡣��Ҫע�⣬���п�������ͬ�� $x$ �� $y$ ����Ϊ Akira �ǳ���ɥ�����ܲ�ֹһ����ͬһ����ͬһ�����⡣

����Լ��� $n$ С�� $1000$��$p_1$ �� $p_2$ С�� $300$�����һ���������㣬�� `0 0 0`����ʾ����Ľ���������Լ���ÿ�����Ե㶼��һ�µģ�û��ì�ܵĴ𰸡�

### �����ʽ
����ÿ�����ݼ�������������㹻����Ϣ�������о�����з��࣬�밴�������������ʥ�����ʶ��ţ�һ��һ�������⣬���������֮�󣬴�ӡ `end` �����һ�С����򣬼�������������ݼ��������㹻����Ϣ��ʶ��������ʥ�ĳ�Ա���������һ���д�ӡ `no`��
### ˵��/��ʾ
���� $100\%$ �����ݣ�ÿ�����ݵ������ 10 �����ݣ�$n<1000$��$p_1,p_2<300$��$1\le x_i, y_i \le p_1+p_2$��

```input1
2 1 1
1 2 no
2 1 no
3 2 1
1 1 yes
2 2 yes
3 3 yes
2 2 1
1 2 yes
2 3 no
5 4 3
1 2 yes
1 3 no
4 5 yes
5 6 yes
6 7 no
0 0 0
```

```output1
no
no
1
2
end
3
4
5
6
end
```

