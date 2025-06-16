## ��Ŀ����
Now here is a matrix with letter 'a','b','c','w','x','y','z' and you can change 'w' to 'a' or 'b', change 'x' to 'b' or 'c', change 'y' to 'a' or 'c', and change 'z' to 'a', 'b' or 'c'. After you changed it, what's the largest submatrix with the same letters you can make?

## �����ʽ
The input contains multiple test cases. Each test case begins with $m$ and $n (1 <m,n< 1000)$ on line. Then come the elements of a matrix in row-major order on m lines each with n letters. The input ends once EOF is met.

## �����ʽ
For each test case, output one line containing the number of elements of the largest submatrix of all same letters.


## ��Ŀ����
### ��Ŀ����

��������һ���� $n$ �У�$m$ �еľ�������ÿ��Ԫ�ض��� `a`��`b`��`c`��`w`��`x`��`y`��`z`���е�һ������������Խ������޴����²�����

- �� `w` �滻Ϊ `a` �� `b`��
- �� `x` �滻Ϊ `b` �� `c`��
- �� `y` �滻Ϊ `a` �� `c`��
- �� `z` �滻Ϊ `a` �� `b` �� `c`��

������������������������ȫ��Ԫ�ض���ͬ���Ӿ����Ԫ�ظ�������Ƕ��٣�

### �����ʽ

**�����ж���������ݡ�**

����ÿ��������ݣ���һ������������ $n,m$���ֱ�����ʼ������С�������

֮��� $n$ �У�ÿ�� $m$ ���ַ�����ʾ��ʼ�ľ���

### �����ʽ

����ÿ��������ݣ����һ�У���ʾ����������������������ȫ��Ԫ�ض���ͬ���Ӿ����Ԫ�ظ��������ֵ��

### ��������

������ľ��������������ӣ�

```
abcw
wccc
```

```input1
2 4
abcw
wxyz
```

```output1
3
```

