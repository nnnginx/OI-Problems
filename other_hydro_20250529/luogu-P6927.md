## 题目描述
You administer a large cluster of computers with hard drives that use various file system types to store data. You recently decided to unify the file systems to the same type. That is quite a challenge since all the drives are currently in use, all of them are filled with important data to the limits of their capacities, and you cannot afford to lose any of the data. Moreover, reformatting a drive to use a new file system may significantly change the drive’s capacity. To make the reformat possible, you will have to buy an extra hard drive. Obviously, you want to save money by minimizing the size of such extra storage.

You can reformat the drives in any order. Prior to reformatting a drive, you must move all data from that drive to one or more other drives, splitting the data if necessary. After a drive is reformatted, you can immediately start using it to store data from other drives. It is not necessary to put all the data on the same drives they originally started on – in fact, this might even be impossible if some of the drives have smaller capacity with the new file system. It is also allowed for some data to end up on the extra drive.

As an example, suppose you have four drives $A$, $B$, $C$, and $D$ with drive capacities $6$, $1$, $3$, and $3$ GB. Under the new file system, the capacities become $6$, $7$, $5$, and $5$ GB, respectively. If you buy only $1$ GB of extra space, you can move the data from drive $B$ there and then reformat drive $B$. Now you have $7$ GB free on drive $B$, so you can move the $6$ GB from drive $A$ there and reformat drive $A$. Finally, you move the six total gigabytes from drives $C$ and $D$ to drive $A$, and reformat $C$ and $D$.

## 输入格式
The input begins with a line containing one integer $n$ ($1 \le n \le 10^6$), which is the number of drives in your cluster. Following this are $n$ lines, each describing a drive as two integers $a$ and $b$, where $a$ is the capacity with the old file system and $b$ is the capacity with the new file system.

All capacities are given in gigabytes and satisfy $1 \le a,b \le 10^9$. (One thousand petabytes should be enough for everyone, right?)

## 输出格式
Display the total extra capacity in gigabytes you must buy to reformat the drives.

## 题目大意
### 题目描述

你有许多电脑，它们的硬盘用不同的文件系统储存数据。你想要通过格式化来统一文件系统。格式化硬盘可能使它的容量发生变化。为了格式化，你需要买额外的硬盘。当然，你想要买容量最小的额外储存设备以便省钱。你可以按任意顺序格式化硬盘。格式化之前，你要把该硬盘上所有数据移到一个或更多的其他硬盘上（可以分割数据）。格式化后，该硬盘可以立刻开始使用。你没有必要把数据放到它原来所在的硬盘上。数据也可以被放到你额外买的硬盘上。举个例子，假设你有4个硬盘A、B、C、D，容量分别为6、1、3、3(GB)。新的文件系统下，它们的容量变为6、7、5、5(GB)。如果你只买1GB额外空间，你可以把B硬盘的数据放过去然后格式化硬盘B。现在你的B硬盘有7GB容量了，那么你就可以把A的数据放过去然后格式化A，最后把C、D的数据放到A上，再格式化C和D。

### 输入格式

第一行一个数 $n(1≤n≤1,000,000)$，表示你的硬盘数。接下来 $n$ 行，每行两个数 $a$ 和 $b$，分别表示该硬盘的原容量和新文件系统下的容量。所有容量都以 GB 为单位，且$1≤a,b≤1,000,000,000$。

### 输出格式

输出如果要格式化所有硬盘，你最少需要购买多少额外空间(GB)。



```input1
4
6 6
1 7
3 5
3 5

```

```output1
1

```

```input2
4
2 2
3 3
5 1
5 10

```

```output2
5

```

## 提示
Time limit: 5000 ms, Memory limit: 1048576 kB. 

 International Collegiate Programming Contest (ACM-ICPC) World Finals 2016

