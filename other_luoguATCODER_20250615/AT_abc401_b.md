# AT_abc401_b [ABC401B] Unauthorized

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc401/tasks/abc401_b

某天，高桥君对某个网站进行了 $N$ 次操作。

第 $i$ 次操作 $(1 \leq i \leq N)$ 由字符串 $S_i$ 表示，属于以下 4 种之一：

- $S_i =$ `login`：高桥君执行登录操作，进入已登录状态。
- $S_i =$ `logout`：高桥君执行登出操作，进入未登录状态。
- $S_i =$ `public`：高桥君访问网站的公开页面。
- $S_i =$ `private`：高桥君访问网站的非公开页面。

当且仅当高桥君在未登录状态下访问非公开页面时，网站会返回**认证错误**。

在已登录状态下重复登录，或在未登录状态下重复登出，不会触发错误。此外，即使发生认证错误，高桥君仍可继续后续操作。

初始时，高桥君处于未登录状态。

请输出 $N$ 次操作中高桥君收到认证错误的总次数。

## 输入格式

输入通过标准输入给出，格式如下：

> $N$  
> $S_1$  
> $S_2$  
> $\vdots$  
> $S_N$

## 输出格式

输出高桥君收到认证错误的总次数。

## 输入输出样例 #1

### 输入 #1

```
6
login
private
public
logout
private
public
```

### 输出 #1

```
1
```

## 输入输出样例 #2

### 输入 #2

```
4
private
private
private
logout
```

### 输出 #2

```
3
```

## 输入输出样例 #3

### 输入 #3

```
20
private
login
private
logout
public
logout
logout
logout
logout
private
login
login
private
login
private
login
public
private
logout
private
```

### 输出 #3

```
3
```

## 说明/提示

### 约束条件

- $1 \leq N \leq 100$
- $N$ 为整数
- $S_i$ 为 `login`、`logout`、`public`、`private` 之一 $(1 \leq i \leq N)$

### 样例解释 1

各操作的结果如下：  
1. 高桥君进入已登录状态；  
2. 访问非公开页面。因当前已登录，不触发错误；  
3. 访问公开页面；  
4. 高桥君进入未登录状态；  
5. 访问非公开页面。因当前未登录，触发认证错误；  
6. 访问公开页面。  
仅在第 5 次操作时收到认证错误，故输出 `1`。

### 样例解释 2

连续访问非公开页面时，每次操作均会触发认证错误。  
需注意：未登录状态下执行登出操作不会触发错误。

翻译由 DeepSeek V3 完成