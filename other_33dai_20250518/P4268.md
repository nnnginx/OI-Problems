## 题目描述
Bessie the cow is surprisingly computer savvy. On her computer in the barn, she stores all of her precious files in a collection of directories; for example:

```
bessie/
  folder1/
    file1
    folder2/
      file2
  folder3/
    file3
  file4
```

There is a single "top level" directory, called bessie.

Bessie can navigate to be inside any directory she wants. From a given directory, any file can be referenced by a "relative path". In a relative path, the symbol ".." refers to the parent directory. If Bessie were in folder2, she could refer to the four files as follows:

```
../file1
file2
../../folder3/file3
../../file4
```

Bessie would like to choose a directory from which the sum of the lengths of the relative paths to all the files is minimized.

## 输入格式
The first line contains an integer N ($2 \leq N \leq 100,000$), giving the total number of files and directories. For the purposes of input, each object (file or directory) is assigned a unique integer ID between 1 and $N$, where ID 1 refers to the top level directory.
Next, there will be $N$ lines. Each line starts with the name of a file or directory. The name will have only lower case characters a-z and digits 0-9, and will be at most 16 characters long. Following the name is an integer, $m$. If $m$ is 0, then this entity is a file. If $m > 0$, then this entity is a directory, and it has a total of $m$ files or directories inside it. Following $m$ there will be $m$ integers giving the IDs of the entities in this directory.

## 输出格式
Output the minimal possible total length of all relative paths to files. Note that this value may be too large to fit into a 32-bit integer.

## 题目大意
### 题目描述

奶牛 Bessie 出人意料地精通计算机。她在谷仓的电脑上将所有珍贵文件存储在一系列目录中；例如：

```
bessie/
  folder1/
    file1
    folder2/
      file2
  folder3/
    file3
  file4
```

有一个单一的“顶级”目录，名为 `bessie`。

Bessie 可以导航到她想要的任何目录。从给定目录中，任何文件都可以通过“相对路径”引用。在相对路径中，符号 `..` 表示父目录。如果 Bessie 在 `folder2` 中，她可以通过以下方式引用四个文件：

```
../file1
file2
../../folder3/file3
../../file4
```

Bessie 希望选择一个目录，使得从该目录到所有文件的相对路径长度之和最小。

### 输入格式

第一行包含一个整数 $N$（$2 \leq N \leq 100,000$），表示文件和目录的总数。为了输入方便，每个对象（文件或目录）被分配一个唯一的整数 ID，范围在 $1$ 到 $N$ 之间，其中 ID $1$ 表示顶级目录。

接下来是 $N$ 行。每行以文件或目录的名称开头。名称仅包含小写字母 `a-z` 和数字 `0-9`，且长度最多为 $16$ 个字符。名称后是一个整数 $m$。如果 $m$ 为 $0$，则该实体是一个文件。如果 $m > 0$，则该实体是一个目录，并且它内部共有 $m$ 个文件或目录。在 $m$ 之后是 $m$ 个整数，表示该目录中实体的 ID。

### 输出格式

输出所有文件的相对路径长度的最小可能总和。请注意，此值可能超过 32 位整数的范围。

### 提示

此输入描述了上面给出的示例目录结构。

最佳解决方案是位于 `folder1` 中。从该目录中，相对路径为：

```
file1
folder2/file2
../folder3/file3
../file4
```

题目来源：Mark Gordon

```input1
8
bessie 3 2 6 8
folder1 2 3 4
file1 0
folder2 1 5
file2 0
folder3 1 7
file3 0
file4 0
```

```output1
42
```

## 提示
This input describes the example directory structure given above.

The best solution is to be in folder1. From this directory, the relative paths are:

```
file1
folder2/file2
../folder3/file3
../file4
```

Problem credits: Mark Gordon

