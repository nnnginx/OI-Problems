# 权限

## 题目描述

奶龙说：一场比赛至少有一个签到题。

奶龙使用 Linux 系统. $\text{chmod}$ 是一个用于更改文件或目录权限的命令, 它是 $\text{Linux}$ 和其他类 $\text{Unix}$ 操作系统中的常用命令之一. $\text{chmod}$ 命令允许用户为文件或目录设置不同的权限, 以控制谁可以读取, 写入或执行这些文件.在 $\text{Linux}$ 系统中, 每个文件或目录都有与之相关联的权限, 这些权限决定了谁可以对文件进行何种操作.用户被分为三类: 所有者 (owner), 所属组 (group) 和其他人 (others). 每类用户又都有读 (`r`), 写 (`w`) 和执行 (`x`) 三种权限. 这 $9$ 种权限可以分别指定. 我们称权限字符串是一个长度为 $9$ 的字符串, 按顺序分别对应以上提到的 $9$ 种权限, 如果具有此权限, 则为 `r`, `w`, `x` 中相应的那一个, 否则为 `-`.

例如权限字符串 `rwxr-x--x` 说明, 该文件对于所有者具有全部权限, 对于所属组用户只具有读和执行权限, 而对于其他人只具有执行权限.

使用 $\text{chmod}$ 命令时, 你可以提供模式串来修改权限. 在本题, 我们只考虑长度为 $3$ 的由不大于 $7$ 的数字组成的模式串, 其三个数字从左往右依次代表所有者 (owner), 所属组 (group) 和其他人 (others) 的权限. 对于每个数字, 其最低三个二进制位从高向低分别表示了该类用户是否具有读 (`r`), 写 (`w`) 和执行 (`x`) 权限. 例如: 执行 `chmod 760 file.txt` 后, 表示文件的权限字符串为 `rwxrw----`.

奶龙现在修改了一个文件的权限，你需要求出修改后文件的权限字符串。

## 输入格式

一行一个整数 $n$ 表示模式串。

## 输出格式

一行字符串，表示权限字符串。

## 样例 #1

### 样例输入 #1

```
777
```

### 样例输出 #1

```
rwxrwxrwx
```

## 样例 #2

### 样例输入 #2

```
760
```

### 样例输出 #2

```
rwxrw----
```

## 提示

对于 $20\%$ 的数据，满足模式串的三位数相等。

对于 $100\%$ 的数据，满足为合法的模式串。