## ��Ŀ����
### Warning: If you submit a malicious program, you will be banned.
### ���棺�����ύ���⽫����š�

## ��Ŀ����
Did you know that the word "robot" is almost 100 years old? It was first introduced in 1920, in the science-fiction theatrical play $R.U.R.$ , written by Karel Capek. As a tribute to this Czech writer, an educational programming language was named Karel many years later at Stanford University. Your task is to implement an interpreter of a simplified version of this programming language.

The Karel programming language controls a robot named Karel, who lives in a grid of unit squares. Some of the squares are free, while others contain a barrier. Karel always occupies one of the free squares and faces one of the four cardinal directions. The two basic commands are "move forward" and "turn left." The language also provides simple conditional and looping statements. The main educational potential of the language lies in the possibility of defining new procedures for more complex tasks.

Our simplified version of the language can be described by the following grammar:

```plain
<program> := "" | <command> <program>
<command> := "m" | "l" | <proc-call> |
             "i" <condition> "(" <program> ")(" <program> ")" |
             "u" <condition> "(" <program> ")"
<condition> := "b" | "n" | "s" | "e" | "w"
<proc-call> := <uppercase-letter>
<proc-def> := <uppercase-letter> "=" <program>
```
There are five types of commands:

- $\texttt m$ ("move forward") advances Karel's position by one grid square in its current heading, unless there is a barrier, in which case the command has no effect.
- $\texttt l$ ("turn left") makes Karel turn left $90$ degrees.
- $\texttt X$ where $\texttt X$ is any uppercase letter, invokes the procedure named $\texttt X$. 
- $\texttt i$ ("if") followed by a single-letter condition, and two programs in parentheses. If the condition is satisfied, the first program is executed. Otherwise, the second program is executed.
- $\texttt u$ ("until") followed by a single-letter condition, and a program in parentheses. If the condition is satisfied, nothing is done. Otherwise, the program is executed and then the command is repeated.

A condition can be either '$b$', which is satisfied if and only if there is a barrier in the next square in Karel's current heading, or one of the four directional letters `n`, `s`, `e`, or `w`, which is satisfied if and only if Karel's current heading is north, south, east, or west, respectively.


For instance, a simple program `ub(m)` can be understood to mean: ��keep moving forward until there is a barrier," while `un(l)` means "turn to the north." A procedure definition `R=lll` defines a new procedure `R` which effectively means "turn right."


## �����ʽ
The first line of input contains four integers $r, c, d$ and $e$, where $r$ and $c$ $(1 \leq r, c \leq 40)$ are the dimensions of the grid in which Karel lives, $d$ $(0 \leq d \leq 26)$ is the number of procedure definitions, and $e$ $(1 \leq e \leq 10)$ is the number of programs to be executed.

Then follow $r$ lines describing the grid (running north to south), each containing c characters (running west to east), each character being either `.` (denoting a free square) or `#` (denoting a barrier). All squares outside this given area are considered barriers, which means Karel may never leave the area.

Each of the next $d$ lines contains a procedure definition, associating a procedure name (one uppercase letter) with a program forming the procedure body. No procedure name is defined more than once. Procedure bodies may contain invocations of procedures that have not yet been defined.

The last $2e$ lines describe the programs to be executed. Each such description consists of a pair of lines. The first line of each pair contains two integers $i$ and $j$ and a character $h$, where $i$ $(1 \leq i\leq r)$ is the row and $j$ $(1 \leq j \leq c)$ is the column of Karel's initial position, and $h \in \{ \texttt n, \texttt s, \texttt e, \texttt w\}$ represents Karel's initial heading. It is guaranteed that the initial position is a free square. The second line of each pair contains a program to be executed from that initial position.

All procedure bodies and all programs to be executed are at least $1$ and at most $100$ characters long, syntactically correct, and only contain invocations of procedures that are defined. The lines with procedure definitions and programs to be executed contain no whitespace characters.


## �����ʽ
For each program execution, output the final position of Karel after the complete program is executed from the respective initial position. Follow the format used to describe initial positions, that is, two numbers and a directional character. If a particular execution never terminates, output `inf` instead.


## ��Ŀ����
## ��Ŀ����

��֪���������ˡ�������Ѿ���100�����ʷ���������������1920��Ŀƻ�Ϸ�硶R.U.R.R.U.R.���У����׶��������д�ġ�Ϊ������λ�ݿ������¾���һ�ֽ�����������ڶ������˹̹����ѧ������ΪKarel������������ʵ�ִ˱�����Լ򻯰汾�Ľ�������

Karel������Կ�����һ������Karel�Ļ����ˣ���������һ����λ����������С�һЩ���������ɵģ�����һЩ��������ϰ�����׶�����ռ��һ�����������Σ������ĸ���������֮һ���������������ǡ���ǰ�ƶ����͡�����ת���������Ի��ṩ�򵥵���������ѭ����䡣�����Ե���Ҫ����Ǳ������Ϊ�����ӵ��������³���Ŀ����ԡ�

���Ǽ򻯵����԰汾�����������﷨������

```
<program> := "" | <command> <program>
<command> := "m" | "l" | <proc-call> |
             "i" <condition> "(" <program> ")(" <program> ")" |
             "u" <condition> "(" <program> ")"
<condition> := "b" | "n" | "s" | "e" | "w"
<proc-call> := <uppercase-letter>
<proc-def> := <uppercase-letter> "=" <program>
```
���������͵����

m������ǰ�ƶ������ڵ�ǰ�����н�Karel��λ����ǰ�ƶ�һ�����񣬳������ϰ������������£�������Ч��

l������ת����ʹ���׶���ת9090�ȡ�

x������x���κδ�д��ĸ��������Ϊx�Ĺ��̡�

i����if�������һ������ĸ�������������������������������������ִ�е�һ�����򡣷���ִ�еڶ�������

u����ֱ�����������һ������ĸ��������������һ����������������㣬��ʲôҲ���������򣬽�ִ�иó���Ȼ���ظ������

���������ǡ�b�������ҽ���Karel��ǰ�������һ�������д����ϰ���ʱ���㣬�����ĸ�������ĸn��s��e��w�е�һ�������ҽ���Karel��ǰ����ֱ�Ϊ�����ϡ�������ʱ���㡣

���磬һ���򵥵ĳ���ub��m���������Ϊ������ǰ����ֱ�����ϰ���Ϊֹ������un��l����ʾ��ת�򱱷�����������R=lll������һ���µĳ���R����ʵ������ζ�š���ת��

����ĵ�һ�а����ĸ�����r��c��dr��c��d��e������r��c��1��r�� c��40����Karel��ס������ĳߴ磬d��0��D��26���ǳ������������e��1����E��10�� ��Ҫִ�еĳ�������

Ȼ���������������r�У��ӱ����ϣ���ÿ������c�ַ���������������ÿ���ַ����ǡ�����ʾ���������Σ���#����ʾ�ϰ������������������й㳡������Ϊ�ϰ������ζ�ſ��׶�������Զ�����뿪������

��������d���е�ÿһ�ж�����һ�����̶��壬���������ƣ�һ����д��ĸ���빹�ɹ�������ĳ����������û�ж�ζ���������ơ�����������ܰ�����δ����Ĺ��̵��á�

�������������Ҫִ�еĳ���ÿ��������������һ������ɡ�ÿ�Եĵ�һ�а�����������ii��jj�Լ�һ���ַ�hh������i��1���ҡ�r�� ���к�j��1����J��c�� ��Karel��ʼλ�õ��У�h��{n��s��e��w}����Karel�ĳ�ʼ���⡣��֤��ʼλ��Ϊ���������Ρ�ÿ�Եĵڶ��а����Ӹó�ʼλ��ִ�еĳ���

����Ҫִ�еĹ���������г���ĳ�������Ϊ11���ַ������Ϊ100100���ַ����﷨��ȷ�����ҽ������Ѷ�����̵ĵ��á�����Ҫִ�еĹ��̶���ͳ�����в������ո��ַ���

�����ʽ

����ÿ������ִ�У��ڴӸ��Եĳ�ʼλ��ִ��������������Karel������λ�á���ѭ����������ʼλ�õĸ�ʽ�����������ֺ�һ�������ַ�������ض�ִ�д�δ��ֹ�����Ϊ���inf��

```input1
4 8 5 7
.......#
..#....#
.###...#
.....###
R=lll
G=ub(B)
B=ub(m)lib(l)(m)
H=ib()(mmHllmll)
I=III
1 1 w
G
1 1 e
G
2 2 n
G
2 6 w
BR
4 1 s
ib(lib()(mmm))(mmmm)
1 1 e
H
2 2 s
I

```

```output1
1 1 w
inf
1 1 w
2 4 s
4 4 e
1 4 e
inf

```

## ��ʾ
Source: ICPC World Finals 2019.

