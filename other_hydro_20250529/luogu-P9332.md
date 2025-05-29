## ��Ŀ����
**����һ�������⡣**

**���ڼ���ԭ�򣬱����ݲ�֧���ύ�����⡣**

**������ܹ��ṩ�ٷ����ݶ�Ӧ�� grader������ @[_RSY_](/user/46197) ��ϵ��**

## ��Ŀ����
**����Ŀ������**

In the factory of JOI Co., Ltd., there are $N$ tables, numbered from $0$ to $N - 1$. In the factory, there are $N - 1$ belt conveyors, numbered from $0$ to $N - 2$. The belt conveyor $i \ (0 \le i \le N - 2)$ connects the table $A_i$ and the table $B_i$. It transports products from one table to the other table. However, we cannot see the direction of transportation. If we ignore the directions of the belt conveyors, every pair of tables is connected by a number of belt conveyors.

IOI-kun is the director of the factory. Since he forgets the direction of transportation of every belt conveyor, he will perform the following sequential operations several times.

1. He chooses a number of belt conveyors, and reverses the directions of transportation of the chosen belt conveyors.
2. He chooses a number of tables, and puts a product on each chosen table.
3. For every table where a product is put, one of the following happens simultaneously.
    - If there is no belt conveyor transporting products from it, nothing happens.
    - If there are belt conveyors transporting products from it, the product on the table is transported by one of such belt conveyors. The product stops at the destination of the belt conveyor. The product will not move anymore.
4. IOI-kun confirms whether there are one or more products on each table. If there are products on a table, IOI-kun takes all of them.
5. For every belt conveyor whose direction is reversed in the operation 1., IOI-kun reverts its direction. Its direction becomes the original direction.

IOI-kun wants to specify the original direction of every belt conveyor by performing the above sequential operations at most $30$ times.

Write a program which, given information of the tables connected by the belt conveyors, implements IOI-kun��s strategy to specify the original direction of every belt conveyor by performing the above sequential operations at most $30$ times.

**��ʵ��ϸ�ڡ�**

You need to submit one file.

The file is `conveyor.cpp`. It should implement the following function. The program should include `conveyor.h` using the preprocessing directive `#include`.

In `conveyor.cpp`, the following function should be implemented.

```cpp
void Solve(int N, std::vector<int> A, std::vector<int> B)
```

This function is called only once for each test case.

- The parameter `N` is the number of tables $N$.
- The parameters `A��B` are arrays of length $N - 1$, describing the tables connected by the belt conveyors.

Your program can call the following function.

```cpp
std::vector<int> Query(std::vector<int> x, std::vector<int> y)
```

Using this function, IOI-kun performs the operations in the factory.

- The parameter `x` is an array of length $N - 1$. For $0 \le \texttt{i} \le N - 2$, IOI-kun reverses the direction of the belt conveyor `i` if `x[i] = 1`, and does not reverses the direction of the belt conveyor `i` if `x[i] = 0`.
- The parameter `y` is an array of length $$. For $0 \le \texttt{j} \le N - 1$, IOI-kun puts a product on the table `j` if `y[j] = 1`, and does not put a product on the table `j` if `y[j] = 0`.
- Let `z` be the return value of this function. It is an array of length $N$. For $0 \le \texttt{j} \le N - 1$, there are one or more products on the table `j` if `z[j] = 1`, and there is no product on the table `j` if `z[j] = 0`.
- The length of the array `x` should be equal to $N - 1$. If this condition is not satisfied, your program is judged as `Wrong Answer [1]`.
- Every element of the array `x` should be `0` or `1`. If this condition is not satisfied, your program is judged as `Wrong Answer [2]`.
- The length of the array `y` should be equal to $N$. If this condition is not satisfied, your program is judged as `Wrong Answer [3]`.
- Every element of the array `y` should be `0` or `1`. If this condition is not satisfied, your program is judged as `Wrong Answer [4]`.
- The function Query should not be called more than $30$ times. If it is called more than $30$ times, your program is judged as `Wrong Answer [5]`.

```cpp
void Answer(std::vector<int> a)
```

Using this function, IOI-kun reports the original direction of each belt conveyor.

- The parameter `a` is an array of length $N - 1$. For $0 \le \texttt{i} \le N - 2$, the belt conveyor `i` transports products from $A_i$ to $B_i$ if `a[i] = 0`, and it transports products from $B_i$ to $A_i$ if `a[i] = 1`.
- The length of the array `a` should be equal to $N - 1$. If this condition is not satisfied, your program is judged as `Wrong Answer [6]`.
- Every element of the array `a` should be `0` or `1`. If this condition is not satisfied, your program is judged as `Wrong Answer [7]`.
- If IOI-kun reports wrong direction of a belt conveyor, your program is judged as `Wrong Answer [8]`.
- The function `Answer` should be called exactly once. If the function `Answer` is called more than once, your program is judged as `Wrong Answer [9]`. When the function `Solve` terminates, if the function `Answer` is not called, your program is judged as `Wrong Answer [10]`.

#### Important Notices

- Your program can implement other functions for internal use, or use global variables.
- Your program must not use the standard input and the standard output. Your program must not communicate with other files by any methods. However, your program may output debugging information to the standard error.

**�����ⷽʽ��**

You can download an archive file from the contest webpage which contains the sample grader to test your program. The archive file also contains a sample source file of your program.

The sample grader is the file `grader.cpp`. In order to test your program, put `grader.cpp`, `conveyor.cpp`, `conveyor.h` in the same directory, and run the following command to compile your programs. Instead, you may run `compile.sh` contained in the archive file.

```plain
g++ -std=gnu++17 -O2 -o grader grader.cpp conveyor.cpp
```

When the compilation succeeds, the executable file `grader` is generated.

Note that the actual grader is different from the sample grader. The sample grader will be executed as a single process, which will read input data from the standard input and write the results to the standard output.

## �����ʽ
The sample grader reads the following data from the standard input.

> $N$
>
> $A_0 \ A_1 \ \cdots \ A_{N - 2}$
>
> $B_0 \ B_1 \ \cdots \ B_{N - 2}$
>
> $C_0 \ C_1 \ \cdots \ C_{N - 2}$

For $0 \le i \le N - 2$, we have $C_i = 0$ if the belt conveyor $i$ transports products from the table $A_i$ to the table $B_i$. Otherwise, we have $C_i = 1$.

## �����ʽ
The sample grader outputs the following information to the standard output (quotes for clarity).

- If your program is judged as correct, it reports the number of function calls to `Query` as `Accepted: 22`.
- If your program is judged as any type of Wrong Answer, the sample grader writes its type as `Wrong Answer [4]`.

If your program satisfies the conditions of several types of Wrong Answer, the sample grader reports only one of them.

In sample grader, among the belt conveyors transporting products from the table where a product is put, the belt conveyor transporting the product is chosen uniformly and randomly determined by pseudorandom numbers whose results do not change for different executions. In order to change the seed of pseudorandom numbers, run the sample grader with the first integer argument as follows.

```plain
./grader 2023
```

## ��Ŀ����
### ��Ŀ����

�� JOI ���޹�˾�Ĺ������ $N$ �����ӣ��� $0$ �� $N-1$ ��š��������� $N-1$ ��Ƥ�����ͻ����� $0$ �� $N-2$ ��š��� $i$ �� $(0 \le i \le N-2)$ Ƥ�����ͻ��������� $A_i$ ������ $B_i$��������Ʒ��һ���������䵽��һ�����ӡ�Ȼ��������**��֪��**����ķ���


IOI-kun �ǹ����ľ���������������ÿ��Ƥ�����ͻ������䷽��������ΰ�������˳��ִ�в�����
1. ѡ�������ʹ�������ת��ѡ���ʹ������䷽��
2. ѡ�������ӣ�����ÿ��ѡ���������Ϸ�һ����Ʒ��
3. ÿ���Ѳ�Ʒ����һ��������ʱ���ͻᷢ���������֮һ��

- ���û�����ʹ�����Ʒ�Ӹ��������ߣ��򲻻ᷢ���κ����顣
- ��������ʹ�����Ʒ�Ӹ��������ߣ��������ϵĲ�Ʒ��������һ�����ʹ����䡣��Ʒ�������ʹ���Ŀ�ĵ�ֹͣ�����Ҳ�Ʒ�������ƶ���
4. IOI-kun ��ȷ��ÿ���������Ƿ��в�Ʒ������в�Ʒ�������ϣ�IOI-kun �������ȫ�����ߡ�
5. ����ÿ���ڲ��� 1 �иı��˷����Ƥ�����ͻ���IOI-kun ���Ὣ�䷽��ָ���ԭ���ķ���IOI-kun ϣ��ͨ�����ִ�� $30$ ������˳�������Ϊÿ��Ƥ�����ͻ�ָ��ԭʼ����

���дһ�����򣬸���Ƥ�����ͻ�֮������ӱ�ʵ�� IOI-kun �Ĳ��ԣ���ͨ�����ִ�� $30$ ������˳�������Ϊÿ��Ƥ�����ͻ�ָ��ԭʼ����

### ʵ��ϸ��

����Ҫʵ��һ�� C++ �����ύʱ**����Ҫ**���� `conveyor.h`��

��Ӧ��ʵ�����º�����

```cpp
void Solve(int N, std::vector<int> A, std::vector<int> B)
```


�ú�������ÿ�����������б�����һ�Σ�

- ���� $N$�����ʹ����ӵ����ӵ�������
- ���� $A$ �� $B$ �ǳ���Ϊ $N - 1$ �����飬������Ƥ�����ͻ����ӵ����ӡ�

���ĳ�����Ե������º�����

```cpp
std::vector<int> Query(std::vector<int> x, std::vector<int> y)
```


ʹ�����������IOI-kun �ڹ�����ִ�в�����

- ���� $x$ ��һ������Ϊ $N - 1$ �����顣���� $0\le i\le N - 2$����� $x_i = 1$��IOI-kun ����ת�� $i$ �����ʹ��ķ��򣬷��򲻷�ת�ô��ʹ��ķ���
- ���� $y$ ��һ������Ϊ $N$ �����顣���� $0 \le j \le N - 1$����� $y_j = 1$��IOI-kun ���ڵ� $j$ �������Ϸ���һ����Ʒ�����򲻻��ڸ������Ϸ��ò�Ʒ��
- �� $z$ �Ǹú����ķ���ֵ������һ������Ϊ $N$ �����顣���� $0 \le j \le N - 1$����� $z_j = 1$����� $j$ ���������в�Ʒ����� $z_j = 0$����� $j$ ��������û�в�Ʒ��
- ���� $x$ �ĳ���Ӧ���� $N - 1$���������������������ĳ��򽫱���Ϊ `Wrong Answer[1]`��
- ���� $x$ �е�ÿ��Ԫ�ض�ӦΪ $0$ �� $1$���������������������ĳ��򽫱���Ϊ `Wrong Answer[2]`��
- ���� $y$ �ĳ���Ӧ���� $N$���������������������ĳ��򽫱���Ϊ `Wrong Answer[3]`��
- ���� $y$ �е�ÿ��Ԫ�ض�ӦΪ $0$ �� $1$������������������������ĳ��򽫱���Ϊ `Wrong Answer[4]`��
- ���� Query ���ֻ�ܱ����� $30$ �Ρ���������ô������� $30$ �Σ����ĳ��򽫱���Ϊ `Wrong Answer[5]`��

```cpp
void Answer(std::vector<int> a)
```

ʹ�����������IOI-kun �ᱨ��ÿ�����ʹ���ԭʼ����

- ���� $a$ ��һ������Ϊ $N - 1$ �����顣���� $0 \le i \le N - 2$����� $a_i = 0$�������ʹ� $i$ ����Ʒ�� $A_i$ ���䵽 $B_i$����� $a_i = 1$���򽫲�Ʒ�� $B_i$ ���䵽 $A_i$��
- ���� $a$ �ĳ��ȱ������ $N - 1$��������������㣬���ĳ��򽫱���Ϊ `Wrong Answer[6]`��
- ���� $a$ �е�ÿ��Ԫ�ض�����Ϊ $0$ �� $1$��������������㣬���ĳ��򽫱���Ϊ `Wrong Answer[7]`��
- ��� IOI-kun ���������ʹ��Ĵ��������ĳ��򽫱���Ϊ `Wrong Answer[8]`��
- ���� `Answer` ���뱻**ǡ�õ���һ��**��������� `Answer` �����ö�Σ����ĳ��򽫱���Ϊ `Wrong Answer[9]`�������� `Solve` ����ʱ��������� `Answer` ��δ�����ã����ĳ��򽫱���Ϊ `Wrong Answer[10]`��

### �����ʽ
��������⽫�������¸�ʽ�����ݣ�
```
N
A[0] A[1] ... A[N - 2]
B[0] B[1] ... B[N - 2]
C[0] C[1] ... C[N - 2]
```
���� $0\le i\le N - 2$������� $i$ �����ʹ��Ὣ��Ʒ�� $A_i$ ������ $B_i$����ô $C_i$ Ϊ $0$������ $C_i$ Ϊ $1$��

### �����ʽ
��������⽫������Ϣ����� stdout��

-�����ĳ����ж�Ϊ��ȷ��������ĺ��� `Query` ���õ�����Ϊ `Accepted: 22` ��

-�����ĳ����ж�Ϊ�κ����͵Ĵ���𰸣���������Ա��������дΪ `Wrong Answer[4]`��



������ĳ������㼸�����͵Ĵ���𰸵������������������ֻ��������һ�֡�

### �����������
#### ���� #1
```plain
3
0 2
2 1
1 0
```

### ˵��/��ʾ
|��������|��������|����ֵ|
|:-|:-|:-|
|`Solve(3, [0, 2], [2, 1])`|||
||`Query([0, 0], [0, 0, 1])`|`[1, 0, 0]`|
||`Query([1, 0], [1, 0, 1])`|`[0, 1, 1]`|
||`Query([1, 1], [0, 0, 1])`|`[0, 0, 1]`|
||`Query([0, 1], [1, 1, 1])`|`[1, 0, 1]`|
||`Answer([1, 0])`||

���ڶ� `Query` �ĵ�һ�ε��ã���һ�����ܵķ���ֵ�� `[0,1,0]`��



���ڶ� `Query` �ĵڶ��ε��ã�λ��Ϊ $0$ �ϵĲ�Ʒͨ�����ʹ� $0$ �����͵�λ�� $2$����ͣ�������ע�⣬�ò�Ʒ���ᱻ���ʹ� $1$ ���͵�λ�� $1$��



ע�⣬���ʾ������**�������κ�������**������������



�·��ļ��У�`sample-02.txt` ���� Subtask $1$ ������������`sample-03.txt` ���� Subtask $2$ ������������

����ĳЩ����������ʵ�ʵ��������**������Ӧ��**������ζ����������ڿ�ʼʱû�й̶��Ĵ𰸣���������ǰ�� `Query` �����ĵ��ý�����Ӧ��

Translate by @[tbdsh](/user/752485).

## ��ʾ
**���������ʾ����**

Here is a sample input for the sample grader and corresponding function calls.

**Sample Input 1:**

```plain
3
0 2
2 1
1 0
```

|Function Calls|Function Calls|Return Values|
|:-|:-|:-|
|`Solve(3, [0, 2], [2, 1])`|||
||`Query([0, 0], [0, 0, 1])`|`[1, 0, 0]`|
||`Query([1, 0], [1, 0, 1])`|`[0, 1, 1]`|
||`Query([1, 1], [0, 0, 1])`|`[0, 0, 1]`|
||`Query([0, 1], [1, 1, 1])`|`[1, 0, 1]`|
||`Answer([1, 0])`||

For the first function call to `Query`, another possible return value is `[0, 1, 0]` other than `[1, 0, 0]`.

For the second function call to `Query`, the product on the table $0$ is transported to the table $2$ by passing through the belt conveyor $0$, and stops there. Note that this product will not be transported to the table $1$ by passing through the belt conveyor $1$.

Note that this sample input **does not satisfy the constraints of any subtask**.

Among the files which can be obtained from the contest webpage, `sample-02.txt` satisfies the constraints of Subtask $1$, and `sample-03.txt` satisfies the constraints of Subtask $2$.

#### Notices for Grading

For some of the test cases, the actual grader is adaptive. This means the grader does not have a fixed answer in the beginning, and responds according to previous function calls to Query. It is guaranteed that there is at least one answer which does not contradict all the responses of the the grader.

**�����ݷ�Χ��**

�������в������ݣ����� $0 \le A_i, B_i \le N - 1$����֤�������д��ʹ��ķ�������л�����ͨ����֤���������Ϊ������

|��������|��ֵ|$N =$|��������|
|:-:|:-:|:-:|:-:|
|$1$|$1$|$2$|��|
|$2$|$14$|$30$|��|
|$3$|$10$|$10 ^ 5$|$A_i = i$��$B_i = i + 1$|
|$4$|$75$|$10 ^ 5$|��|

