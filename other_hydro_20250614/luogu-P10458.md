## ��Ŀ����
A fractal is an object or quantity that displays self-similarity, in a somewhat technical sense, on all scales. The object need not exhibit exactly the same structure at all scales, but the same "type" of structures must appear on all scales.

A box fractal is defined as below :

-  A box fractal of degree $1$ is simply X
-  A box fractal of degree $2$ is
```
X X
 X
X X
```
- If using $B(n - 1)$ to represent the box fractal of degree $n - 1$, then a box fractal of degree $n$ is defined recursively as following
```
B(n - 1) B(n - 1)
     B(n - 1)
B(n - 1) B(n - 1)
```
Your task is to draw a box fractal of degree $n$.

## �����ʽ
The input consists of several test cases. Each line of the input contains a positive integer $n$ which is no greater than $7$. The last line of input is a negative integer $-1$ indicating the end of input.

## �����ʽ
For each test case, output the box fractal using the 'X' notation. Please notice that 'X' is an uppercase letter. Print a line with only a single dash after each test case.

## ��Ŀ����
**����Ŀ������**

�������ڸ��ֳ߶�����ĳ�ּ�����������ʾ�������ԵĶ����������������Ҫ�����г߶���չ����ȫ��ͬ�Ľṹ���������г߶��ϱ��������ͬ�ġ����͡��ṹ��

���ӷ��ζ������£�

- ��Ϊ $1$ �ĺ��ӷ��μ򵥵��� X
- ��Ϊ $2$ �ĺ��ӷ�����
```
X X
 X
X X
```
- ����� $B(n - 1)$ ��ʾ��Ϊ $n - 1$ �ĺ��ӷ��Σ���ô��Ϊ $n$ �ĺ��ӷ��ο��Եݹ�ض�������
```
B(n - 1) B(n - 1)
     B(n - 1)
B(n - 1) B(n - 1)
```
��������ǻ��ƶ�Ϊ $n$ �ĺ��ӷ��Ρ�

**�������ʽ��**

�������������������������ÿһ�а���һ�������� $7$ �������� $n$����������һ����һ�������� $-1$����ʾ����Ľ�����

**�������ʽ��**

����ÿ������������ʹ�� 'X' ����������ӷ��Ρ���ע�⣬'X' ��һ����д��ĸ����ÿ����������֮���ӡһ�н������������ۺš�

���������ڣ�ChatGPT��

```input1
1
2
3 
4 
-1
```

```output1
X
-
X X
 X 
X X
-
X X   X X
 X     X 
X X   X X
   X X   
    X    
   X X   
X X   X X
 X     X 
X X   X X
-
X X   X X         X X   X X
 X     X           X     X 
X X   X X         X X   X X
   X X               X X   
    X                 X    
   X X               X X   
X X   X X         X X   X X
 X     X           X     X 
X X   X X         X X   X X
         X X   X X         
          X     X          
         X X   X X         
            X X            
             X             
            X X            
         X X   X X         
          X     X          
         X X   X X         
X X   X X         X X   X X
 X     X           X     X 
X X   X X         X X   X X
   X X               X X   
    X                 X    
   X X               X X   
X X   X X         X X   X X
 X     X           X     X 
X X   X X         X X   X X
-

```

