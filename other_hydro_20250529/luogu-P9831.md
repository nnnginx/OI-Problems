## ��Ŀ����
Your git project (you don't need to be familiar with git to solve this problem) has some files that should be ignored from synchronizing. You need to calculate the minimum number of lines needed for gitignore.

Formally, your project is a folder. A folder can have files and sub folders. There are no empty folders (i.e. folders without any files or sub folders inside). Initially, the git software will synchronize all the files in your project. However, you can specify some files and folders in the settings (which is called gitignore) to exclude them from synchronizing. For each line in gitignore, you can specify either a file or all the files in a folder. You can $\textbf{not}$  ignore the whole project folder (i.e. an empty line in gitignore).

You are given paths for all the files in the project and whether they should be ignored or shouldn't. Your task is to calculate the minimum number of lines for gitignore.

## �����ʽ
The input contains several test cases. The first line contains a single positive integer $T$ which is the number of test cases. For each test case, you are first given two non-negative numbers $n$ and $m$. And then $n$ non-empty lines of file paths that should be $\textbf{ignored}$, and $m$ non-empty lines of file paths that should $\textbf{not}$ be ignored.

The paths are strings containing lower-cased English alphabets and slashes (`/`) only. Slashes are used to separate folders, sub folders and file name. For exapmle, ``a/b/c/d`` indicates folder ``a`` in the project folder, folder ``b`` in folder ``a``, folder ``c`` in ``b`` and file ``d`` in folder ``c``. All the paths are valid, specifically:

- The path is non-empty and it always indicates a file (i.e. the path does not end with a slash).
- The path does not start with a slash.
- Folder names and file names are non-empty (i.e. there are no consecutive slashes).
- File paths are always unique (i.e. all the paths in a test case are different).
- In a folder, no sub folders and files share the same names. For example, there won't be two files ``a/b/a`` and ``a/b/a/d`` in one test case. However, files ``a/b/a`` and ``a/b/b`` are allowed.

$1\leq n+m\leq 100$ holds and in the whole input there are no more than $1,000$ characters in file paths (i.e. the sum of lengths of file path strings in the whole input file is no more than $1,000$).

## �����ʽ
$T$ lines of non-negative integers, the minimum number of gitignore lines for each test case.

## ��Ŀ����
��ʹ�� git �����һ����Ŀ��һЩ��Ҫ�����Ե��ļ�������Ҫ���� .gitignore �ļ�������д������С�

��ϸ��˵�������Ŀ��һ���ļ��У��ļ��п��Ժ����ļ������ļ��С��ڱ����У�������ֿ��ļ��У������ļ������ļ��е��ļ��У���git �����ͬ������Ŀ�����е��ļ������ǣ�������� .gitignore ��д��һЩ��Ϣ��ʹĳЩ�ļ����ļ��в���ͬ������ .gitignore �ļ��е�һ�У������ָ��һ���ļ�����һ���ļ��У�ʹ������ļ�������ļ����е������ļ�����ͬ����**�㲻���Ժ���������Ŀ�ļ��С�**

���õ���Ŀ�������ļ���·�����Լ������Ƿ�Ӧ�ñ�ͬ������������Ǽ��� .gitignore �ļ������ٵ�������

```input1
2
3 0
data/train
data/test
model
3 1
data/train
data/test
model
data/sample
```

```output1
2
3
```

## ��ʾ
In the first sample test case, the corresponding gitignore file contains $2$ lines: a folder line ``data/`` and a file name ``model``.

In the second sample test case, the corresponding gitignore file contains $3$ file lines: ``data/train``, ``data/test`` and ``model``.

