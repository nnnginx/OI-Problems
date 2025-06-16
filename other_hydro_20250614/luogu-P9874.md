## ��Ŀ����
While most people love to play Wordle these days, Prof. Pang has become addicted to String-dle.

String-dle is an interesting string-guessing game where the player tries to guess a string of $k$ capital letters through several rounds. In each round, the player submits a string of length $k$ as his guess, and the system grades the guess through the following pseudo-code:

```
def grading(answer, guess):
  let count be a hash map
  for i = 1 to k:
    if answer[i] not in count:
      count[answer[i]] = 1
    else:
      count[answer[i]] = count[answer[i]] + 1
  let grade be an array of length k
  for i = 1 to k:
    if answer[i] == guess[i]:
      grade[i] = 'O'
      count[guess[i]] = count[guess[i]] - 1
  for i = 1 to k:
    if answer[i] != guess[i]:
      if count[guess[i]] > 0:
        grade[i] = '-'
        count[guess[i]] = count[guess[i]] - 1
      else:
        grade[i] = 'x'
  return grade
```

The grade consisting of $\tt{O}$ (capital letter O), $\tt{-}$ (dash), and $\tt{x}$ (small letter x) is then returned to the player, and the player may base his next guess on the previous grades. The following is an example of one game Prof. Pang played:

```
G: CRANE
A: xx--x
G: UTTER
A: xxOxx
G: NASAL
A: OOxOO
G: NATAL
A: OOOOO
```

Strings after $\tt{G}$ are Prof. Pang's guesses and strings after $\tt{A}$ are the grades of the guesses. 

Prof. Pang really enjoys the game. He believes that he has developed a perfect strategy for it. However, today he goes mad because he thinks the grading system is bugged! He wants to have someone write an analysis program to figure out the number of possible strings that can be the answer to the puzzle based on his list of guesses and grades.

Since the grading system might be bugged, it might not conform to the pseudo-code given above. So specifically, the task is to find how many strings that are consistent with the input. A string s is consistent with the input if for any guess g in the input and its corresponding grade d, grading(s, g)=d.

And of course, you will be doing the programming.

## �����ʽ
The first line consists of two integers $n$ and $k$ $(1 \le n \le 10^4, 1 \le k \le 19)$, which are the number of guesses and the length of the string, respectively.

The following lines consist of the guesses and the grades, one per line, correspondingly.

## �����ʽ
An integer, denoting how many possible answers there are, modulo $10^9+7$.

## ��Ŀ����
### ��Ŀ����
��������˶��������� Wordle ��ʱ���ӽ���ȴ�Ѿ��������� String-dle �ˡ�

String-dle ��һ����Ȥ�Ĳ��ַ�������Ϸ����������ʱ��Ҫͨ�����ֳ��ԣ��³�һ������Ϊ $k$ ���ַ�����������ÿ�ֳ����У����Ҫ�ύһ������Ϊ $k$ ���ַ�������Ϊ���Ĳ²⣬��ϵͳͨ������α������Ϊ�ύ�Ĳ²�������
```
def grading(answer, guess):
  let count be a hash map
  for i = 1 to k:
    if answer[i] not in count:
      count[answer[i]] = 1
    else:
      count[answer[i]] = count[answer[i]] + 1
  let grade be an array of length k
  for i = 1 to k:
    if answer[i] == guess[i]:
      grade[i] = 'O'
      count[guess[i]] = count[guess[i]] - 1
  for i = 1 to k:
    if answer[i] != guess[i]:
      if count[guess[i]] > 0:
        grade[i] = '-'
        count[guess[i]] = count[guess[i]] - 1
      else:
        grade[i] = 'x'
  return grade
```
���ص��������� $\tt{O}$����д��ĸ O����$\tt{-}$�����ۺţ��� $\tt{x}$��Сд��ĸ x��������ҿ��Ի�����ǰ������������һ�β²⡣�������ӽ������һ����Ϸʾ����
```
G: CRANE
A: xx--x
G: UTTER
A: xxOxx
G: NASAL
A: OOxOO
G: NATAL
A: OOOOO
```
���ַ��� $\tt{G}$ ��������ӽ��ڵĲ²⣬�Լ����ַ��� $\tt{A}$ ������Ǹôβ²��������

�ӽ��ڷǳ�ϲ�������Ϸ����ȷ�����Ѿ�֪���������Ϸ���������ԡ�Ȼ��������������������Ϊ����Ϊ����ϵͳ�������⣡��������дһ���������򣬸������Ĳ²��������ҳ����п��ܵĿ�����Ϊ�𰸵��ַ�����

��������ϵͳ���ܳ������⣬���������ܲ��ٷ������������α���롣������˵������Ҫ�ҵ����з���������ַ�����һ������������ַ�����ָ����������������һ���²�  $g$ ��������ȷ���� $d$��������  `grading(s, g)=d`��

��Ȼ����������������

### �����ʽ

��һ������������ $n$��$k$ $(1 \le n \le 10^4, 1 \le k \le 19)$���ֱ��ǲ²�Ĵ������ַ����ĳ��ȡ�

���湲�� $2n$ �У�ÿ���ж���Ӧһ���²������Ӧ��������

### �����ʽ

һ����������ʾ�ж����ֿ��ܵĴ𰸣���ģ $10^9+7$.

### ���� #1

#### �������� #1

```
2 5
CRANE
xx--x
NASAL
OOxOO
```

#### ������� #1

```
21
```

### ���� #2

#### �������� #2

```
1 5
BBBAA
xxxx-
```

#### ������� #2

```
0
```

### ���� #3

#### �������� #3

```
2 5
ABCDE
-xxxx
ABCDE
xxxxx
```

#### ������� #3

```
0
```

### ���� #4

#### �������� #4

```
1 3
ABC
---
```

#### ������� #4

```
2
```

### ���� #5

#### �������� #5

```
1 15
AAAAAAAAAAAAAAB
-xxxxxxxxxxxxxx
```

#### ������� #5

```
918547951
```

## ���� #6

#### �������� #6

```
1 15
AAAAAAAAAAAAAAA
-xxxxxxxxxxxxxx
```

#### ������� #6

```
0
```

### ���� #7

#### �������� #7

```
1 1
K
x
```

#### ������� #7

```
25
```

### ��ʾ

���ڵڶ�������:

������� $\tt{ACDEF}$���� $\tt{BBBAA}$ ������Ϊ $\tt{xxx-x}$.

```input1
2 5
CRANE
xx--x
NASAL
OOxOO
```

```output1
21
```

```input2
1 5
BBBAA
xxxx-
```

```output2
0
```

```input3
2 5
ABCDE
-xxxx
ABCDE
xxxxx
```

```output3
0
```

```input4
1 3
ABC
---
```

```output4
2
```

```input5
1 15
AAAAAAAAAAAAAAB
-xxxxxxxxxxxxxx
```

```output5
918547951
```

```input6
1 15
AAAAAAAAAAAAAAA
-xxxxxxxxxxxxxx
```

```output6
0
```

```input7
1 1
K
x
```

```output7
25
```

## ��ʾ
For the second example:

If the answer is $\tt{ACDEF}$, the guess $\tt{BBBAA}$ will produce a grade of $\tt{xxx-x}$.

