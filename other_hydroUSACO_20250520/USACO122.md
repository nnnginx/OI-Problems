## 题目描述  
一块N x N（1<=N<=10）正方形的黑白瓦片的图案要被转换成新的正方形图案。写一个程序来找出将原始图案按照以下列转换方法转换成新图案的最小方式：  
  
1：转90度：图案按顺时针转90度。  
2：转180度：图案按顺时针转180度。  
3：转270度：图案按顺时针转270度。  
4：反射：图案在水平方向翻转（以中央铅垂线为中心形成原图案的镜像）。  
5：组合：图案在水平方向翻转，然后再按照1到3之间的一种再次转换。  
6：不改变：原图案不改变。  
7：无效转换：无法用以上方法得到新图案。  
  
如果有多种可用的转换方法，请选择序号最小的那个。  
只使用1--7中的一个步骤来完成这次转换。  
  
## 输入格式：  
第一行： 单独的一个整数N。  
第二行到第N+1行： N行每行N个字符（不是“@”就是“-”）；这是转换前的正方形。  
第N+2行到第2*N+1行： N行每行N个字符（不是“@”就是“-”）；这是转换后的正方形。  
## 输出格式：  
单独的一行包括1到7之间的一个数字（在上文已描述）表明需要将转换前的正方形变为转换后的正方形的转换方法。  
## 输入样例#1：   
```  
3  
@-@  
---  
@@-  
@-@  
@--  
--@  
```  
输出样例#1：   
```  
1  
```  