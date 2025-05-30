

## 题目描述
编辑数学公式总是一件烦人的事情，为此HURRICANE小组准备出一个编辑数学公式的软件。除了基本功能外，软件还将实现分式和矩阵输入。按照设想，软件应该是符合人性化设计的，必须最大限度的方便用户输入，尽管代价是软件开发极其复杂。幸好输入的方式和格式都已定好，你只需要编个处理程序就行了，下面是相关的约定和格式

### 格式控制的概念
#### 元素
元素可以是运算符、括号、数字、字母、矩阵、分式。
- 数字: ’0’-’9’ ’.’
- 字母: ’A’-’Z’ ’a’-’z’
- 括号: ’(’ ’)’
保证只占一行且是对齐行。

#### 表达式
由0个到至多500个元素构成的序列。其中矩阵与分式元素总个数最多不超过30个。

#### 编辑框
一个输入表达式的矩形区域。每一个编辑框都包括一个对齐行用作编辑框相互之间的对齐。且我们定义编辑框的宽度为最长一行的字符个数，例如表达式空的时候为0，高度为最高行与最低行之间相差的行数（包括），但最小为1，即使表达式为空。

#### 对齐行
编辑框或元素中某一特定行。该行用于框内对齐表达式及框间对齐，对齐时需要使表达式中的元素的对齐行位于编辑框的对齐行上。

#### 运算符
包括’+’、’-’、’*’、’/’四个，为了区分“-”（减号）与分数线，“-”两边分别加上一个空列。

#### 矩阵
一个 （ ,_ ）的矩阵包含 个编辑框将矩阵分为了m个编辑列和n个编辑行。在矩阵的同一编辑行中，相邻的两个编辑框按编辑框的对齐行对齐，同一编辑列的编辑框按照它们的宽度居中对齐。且必须保证行与行之间至少存在一个空行，列与列之间至少存在一个空列。第一列左边与最后一列右边每行各有一个“[”和“]”，位于各行表达式的对齐行上，如图所示：

#### 分式
分式由分子和分母两个编辑框以及它们之间的分数线组成。分式分数线为一条由“-”组成的字符序列，同时它也是分式的对齐行。分式的宽度为两个编辑框宽度的最大值加2，即在左右两边分别加上一个“-”；而高度为两个编辑框的高度加上分数线的高度1。两个编辑框按居中对齐，如图：  
![分式图例](./2100/file/分式图例.png)

在居中对齐时，如果不能正好对准，则往左偏半格，如上图左边的分母编辑框。


##  **【光标控制】** 
** ** 
**应该指出，编辑框是可以层层嵌套的，比如一个编辑框内有一个矩阵，矩阵内又有若干个编辑框。我们说该编辑框比矩阵的编辑框高一级，矩阵内的所有编辑框同级，分式的两个编辑框也是同级的。 **注意：** 同级只是对一个矩阵或一个分式内的编辑框而言。** 
**光标可以跳到编辑框的开始和末尾，也可以向四个方向移动，设光标所处的最低一级的编辑框为 **A** 。** 
** ** 
**Ø**         **如果光标跳到编辑框的开始（末尾），则把光标置于 **A** 的前端（末端）；** 
** ** 
**Ø**         **当光标上下移动时** 
**n**          **如果 **A** 上 **(** 下 **)** 方有与 **A** 同级的编辑框 **B** ，则把光标置于 **B** 的前端，** 
**示例**|**下移一次后**|
:-:|:-:|
** ** XXXX** |** 
**------** 
** **  XX** ****XXXX** 
**------** 
** **  ** | **XX** **
**示例****下移一次后**
** ** XXXX** |** 
**------** 
** **  XX** ****XXXX** 
**------** 
** **  ** | **XX** **
**n**          **否则对比 **A** 高一级的编辑框作同样判断，若 **A** 是最高级别的编辑框，则不作任何处理。如图，竖线代表光标：** 
**示例**|**下移一次后**|**再下移一次后（不变）**|
:-:|:-:|:-:|
** **  d** ** 
** ** ---** ** 
** **  ** | **c** ** 
**-----** 
** **  a** ** 
** ** ---** ** 
** **  b** **** **  d** ** 
** ** ---** ** 
** **  c** ** 
**-----** 
** **  a** ** 
** ** ---** ** 
** **  b** **** **  d** ** 
** ** ---** ** 
** **  c** ** 
**-----** 
** **  a** ** 
** ** ---** ** 
** **  b** **
**示例****下移一次后****再下移一次后（不变）**
** **  d** ** 
** ** ---** ** 
** **  ** | **c** ** 
**-----** 
** **  a** ** 
** ** ---** ** 
** **  b** **** **  d** ** 
** ** ---** ** 
** **  c** ** 
**-----** 
** **  a** ** 
** ** ---** ** 
** **  b** **** **  d** ** 
** ** ---** ** 
** **  c** ** 
**-----** 
** **  a** ** 
** ** ---** ** 
** **  b** **
** ** 
**Ø**         **当光标左（右）移动时** 
**n**          **若光标位于 **A** 的前端 **(** 末端 **)** ，** 
**u**        **如果左 **(** 右 **)** 边没有同级的编辑框，则光标将返回到更高一级的编辑框（若无则不作处理），置于矩阵或分式的左 **(** 右 **)** 边；** 
**u**        **如果左 **(** 右** 
## 输入格式
**每行有一个代表事件的字符串，直到文件结束。我们约定矩阵的规模不超过** </v:formulas><o:lock v:ext="edit" aspectratio="t"></o:lock>** ** </v:shapetype> **，总的元素个数不超过 **10,000** 。** 
## 输出格式
**按规定的格式输出编辑框的结果，空白的地方用空格补上，每行行末不能有多余空格。最后一行行末保留一个回车。** 
输入样例
输出样例

```input1```

```output1```

## 提示
没有写明提示
## 题目来源
没有写明来源


