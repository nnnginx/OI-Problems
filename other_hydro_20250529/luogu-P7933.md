## 题目描述
小 Frane 已经十年级了，但是在信息课上学习 Pascal 仍然很吃力。老师写下了如下的 Pascal 程序作为家庭作业，他需要根据输入的整数 $N$ 来判断程序的输出。

```pascal
readln(N);
counter := 0;
for i := N-1 downto 1 do begin
	counter := counter + 1;
	if N mod i = 0 then break;
end;
writeln(counter); 
```

请您编写一个程序来解决这个问题。

## 输入格式
一行，一个整数 $N$。

## 输出格式
一行，表示以上程序的输出结果。

```input1
1
```

```output1
0
```

```input2
10
```

```output2
5
```

```input3
27
```

```output3
18
```

## 提示
对于 $100\%$ 的数据，$1\le N\le10^9$。

本题分值按照原比赛设置，满分 $30$ 分。

