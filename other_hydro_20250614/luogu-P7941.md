## ��Ŀ����
Nitori is learning postfix expressions. She has a incomplete postfix expression $E$ of length $n$. Being a Youkai, she wants to find its magical property.

Her postfix expression contains the Bitwise Or operator (denoted as `|`), the Bitwise And operator (denoted as `&`), and numbers `0` and `1`. Being incomplete, some operators have not been decided yet and are denoted as `?`. She promised that $E$ **will become a *vaild* postfix expression** after you complete it.

In this problem, the term *substring* is defined as a continuous segment of $E$. **Two substrings are considered different as long as their positions or length differ.**  So `1?0`, `01?0` are all substrings of `01?01?|`  , but `0101` is not.

Nitori found out that a substring of her expression is *magical* if and only if the following conditions are met:

- It is possible to transform it into a *valid* postfix expression after replacing `?` with either `&` or `|` .
- Among these transformations, it is possible to find at least one of them that after applying it, the expression yields $0$,  and at least one of them that after applying it, the expression yields $1$.

Your task is to find out the number of *magical* substrings.


## �����ʽ
The first line contains an integer $T$, the number of test cases.

For each test case, input one integer $n$ and an expression $E$ in a single line.

## �����ʽ
For each test case, print one integer which is the answer.

## ��Ŀ����
����һ���Ϸ��ĺ� `|&?01` �ĺ�׺���ʽ�����ַ�����ʽ��������Ϊ���Ϸ��ġ��������� `?` �滻Ϊ�����������Ϊһ���Ϸ��ĺ�׺���ʽ������������ж��ٸ��Ӵ����㣺

- �����е� `?` �滻�� `|` �� `&` �󣬸ô�Ϊ�Ϸ��ĺ�׺���ʽ��
- ����һ�ֽ����е� `?` �滻�� `|` �� `&` �ķ���ʹ�ø�ʽ���ý��Ϊ $0$��ͬʱҲ�����滻����ʹ�ý��Ϊ $1$��

������������Ӵ��������������Ӵ��ǲ�ͬ�Ľ������ǳ��Ȳ�ͬ��λ�ò�ͬ��

```input1
2
3 01?
7 01?01?|
```

```output1
1
3
```

## ��ʾ
### Constraints

$1\le T,n\le 2\times 10^6$. The sum of $n$ of all test cases $\le 2\times 10^6$.

