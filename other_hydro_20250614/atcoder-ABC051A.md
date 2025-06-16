## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc051/tasks/abc051_a

イルカは、新年に長さ $ 19 $ の文字列 $ s $ を受け取りました。  
 文字列 $ s $ の形式は `[英小文字 $ 5 $ 文字],[英小文字 $ 7 $ 文字],[英小文字 $ 5 $ 文字]` で表されます。  
 イルカは、カンマで区切られた文字列 $ s $ を、スペースで区切られた文字列に変換したいと思っています。  
 イルカの代わりに、この処理を行うプログラムを作ってください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ s $

## 输出格式
処理した後の文字列を出力せよ。

## 题目大意
### **题目描述**
海豚们的语言总爱在一个单词后面加一个,(英文逗号)已知他们的说话的格式是
```
[5个小写字母]，[7个小写字母]，[5个小写字母]
```
你知道人类的语言是不会再单词后面加逗号的，所以请你
把海豚语言转换成人类的语言。
### **输入格式**
一行，一个字符串s。
### **输出格式**
一行，转换后的语言。
### **输入样例1**
```
happy,newyear,enjoy
```
### **输出样例1**
```
happy newyear enjoy
```
### **输入样例2**
```
haiku,atcoder,tasks
```
### **输出样例2**
```
haiku atcoder tasks
```
### **输入样例3**
```
abcde,fghihgf,edcba
```
### **输出样例3**
```
abcde fghihgf edcba
```

```input1
happy,newyear,enjoy
```

```output1
happy newyear enjoy
```

```input2
haiku,atcoder,tasks
```

```output2
haiku atcoder tasks
```

```input3
abcde,fghihgf,edcba
```

```output3
abcde fghihgf edcba
```

## 提示
### 制約

- $ s $ の長さは $ 19 $ である。
- $ s $ の $ 6 $ 文字目と $ 14 $ 文字目は `,` である。
- それら以外の $ s $ の文字は英小文字である。

### Sample Explanation 1

`happy,newyear,enjoy` に含まれるカンマをスペースで置き換えて、`happy newyear enjoy` を出力します。

