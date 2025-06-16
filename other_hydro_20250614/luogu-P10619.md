## ��Ŀ����
![](https://cdn.luogu.com.cn/upload/image_hosting/hb9vxjp8.png)

## ��Ŀ����
The term ��Harvard architecture�� applies to a computer that has physically separate memories for instructions and data. The term originated with the Harvard Mark I computer, delivered by IBM in 1944, which used paper tape for instructions and relays for data.

Some modern microcontrollers use the Harvard architecture �C but not paper tape and relays! Data memory is organized in banks, each containing the same number of data items. Each data-referencing instruction has a byte offset $f$ to a bank, and a bit $a$ that is used to select the bank to be referenced. If $a$ is $0$, then bank $0$ is referenced. If $a$ is $1$, then the value in a *bank select register* (BSR) identifies the bank to be used. Assume each instruction takes the same time to execute, and there is an instruction that can set the BSR��s value.

For example, suppose there are $4$ banks of $8$ bytes each. To access location $5$, either use a single instruction with $a = 0$ and $f = 5$, or set the BSR to $0$ in one instruction and then use an instruction with $a = 1$ and $f = 5$. The first approach is faster since it does not require setting the BSR.

Now suppose (with the same memory) the location to access is $20$. Only one approach will work here: execute an instruction that sets the BSR to $2$ (unless the BSR already has the value $2$) and then use an instruction with $a = 1$ and $f = 4$.

A program is a sequence of operations. Each operation is either

- a variable reference, written as V$i$, where $i$ is a positive integer, or
- a repetition, written as R$n$ `<program>` E, where $n$ is a positive integer and `<program>` is an arbitrary program. This operation is equivalent to n sequential occurrences of `<program>`.

Your problem is to determine the minimum running time of programs. In particular, given the number and size of the memory banks and a program to be executed, find the minimum number of instructions (which reference memory location and possibly set the BSR) that must be executed to run the program. To do this you must identify a mapping of variables to memory banks that yields the smallest execution time, and report that execution time �C that is, the number of memory references and BSR register settings required. The BSR��s value is initially undefined, and changes only when an instruction explicitly sets its value.

## �����ʽ
The input consists of a single test case. A test case consists of two lines. The first line contains two integers $b$ and $s$, where $1 \leq b \leq 13$ is the number of memory banks and $1 \leq s \leq 13$ is the number of variables that can be stored in each memory bank. The second line contains a non-empty program with at most $1 000$ space-separated elements (each R$n$, V$i$, and E counts as one element).

You may assume the following:
- In a repetition R$n$, the number of repetitions satisfies $1 \leq n \leq 10^6$.
- In a loop operation R$n$ `<program>` E, the loop body `<program>` is not empty.
- In a variable reference V$i$, the variable index satisfies $1 \leq i \leq \min(b \times s, 13)$.
- The total number of variable references performed by an execution of the program is at most $10^{12}$.

## �����ʽ
Display the minimum number of instructions that must be executed to complete the program.

## ��Ŀ����
**����Ŀ������**

������ܹ���һ��������ָ������ݾ��������Ϸֿ��Ĵ洢���ļ��������������Դ�ڹ��� Mark I ��������� IBM �� 1944 �꽻�����ü����ʹ��ֽ����Ϊָ�ʹ�ü̵�����Ϊ���ݡ�

һЩ�ִ�΢������ʹ�ù���ܹ���������ʹ��ֽ���ͼ̵��������ݴ洢������֯�ɶ���洢����bank����ÿ���洢��������ͬ�����������ÿ���������ݵ�ָ���һ���ֽ�ƫ���� $f$ ��һ��λ $a$������ѡ��Ҫ���õĴ洢������� $a$ Ϊ $0$�������ô洢�� $0$����� $a$ Ϊ $1$������*�洢��ѡ��Ĵ���*��BSR���е�ֵ��ʶҪʹ�õĴ洢��������ÿ��ָ��ִ��ʱ����ͬ�����Ҵ��ڿ������� BSR ֵ��ָ�

���磬������ $4$ ���洢����ÿ���洢���� $8$ ���ֽڡ�Ҫ����λ�� $5$������ʹ�� $a = 0$ �� $f = 5$ �ĵ���ָ�������һ��ָ���н� BSR ����Ϊ $0$��Ȼ��ʹ�� $a = 1$ �� $f = 5$ ��ָ���һ�ַ������죬��Ϊ������Ҫ���� BSR��

���ڼ��裨ʹ����ͬ�Ĵ洢����Ҫ���ʵ�λ���� $20$������ֻ��ʹ��һ�ַ�����ִ��һ��ָ� BSR ����Ϊ $2$������ BSR �Ѿ��� $2$����Ȼ��ʹ�� $a = 1$ �� $f = 4$ ��ָ�

�����ǲ��������С�ÿ������������

- �������ã�д�� V$i$������ $i$ ������������
- �ظ���д�� R$n$ `<program>` E������ $n$ ����������`<program>` ��������򡣴˲����൱�� `<program>` �� n ���������֡�

���������ȷ���������С����ʱ�䡣������˵�������ڴ�洢���������ʹ�С�Լ�Ҫִ�еĳ����ҳ�����ִ�е���Сָ�����������ڴ�λ�úͿ������� BSR���������г���Ϊ�ˣ������ȷ��������ӳ�䵽�洢���ķ�ʽ���Բ�����С��ִ��ʱ�䣬�������ִ��ʱ�䡪������ɳ���������ڴ����ú� BSR �Ĵ������õ�������BSR ��ֵ���δ���壬����ָ����ʽ������ֵʱ���ġ�

**�������ʽ��**

�������һ���������������������������С���һ�а����������� $b$ �� $s$������ $1 \leq b \leq 13$ �Ǵ洢����������$1 \leq s \leq 13$ ��ÿ���洢�����Դ洢�ı��������ڶ��а���һ���ǿճ��������� $1 000$ ���ÿո�ָ���Ԫ�أ�ÿ�� R$n$, V$i$ �� E ������һ��Ԫ�أ���

����Լ������¼��㣺
- ���ظ� R$n$ �У��ظ��������� $1 \leq n \leq 10^6$��
- ��ѭ������ R$n$ `<program>` E �У�ѭ���� `<program>` ��Ϊ�ա�
- �ڱ������� V$i$ �У������������� $1 \leq i \leq \min(b \times s, 13)$��
- ����ִ�е��ܱ������������Ϊ $10^{12}$��

**�������ʽ��**

��ʾ��ɳ�������ִ�е���Сָ������

���������ڣ�[ChatGPT](https://chatgpt.com/)��


```input1
1 2
V1 V2 V1 V1 V2
```

```output1
5
```

```input2
2 1
V1 V2 V1 V1 V2
```

```output2
6
```

```input3
1 2
R10 V1 V2 V1 E
```

```output3
30
```

```input4
4 1
V1 R2 V2 V4 R2 V1 E V3 E
```

```output4
17
```

