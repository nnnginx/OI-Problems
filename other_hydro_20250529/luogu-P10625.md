## 题目描述
Anatoly Cheng McDougal is a typical student in many ways. Whenever possible he tries to cut and paste code instead of writing it from scratch. Unavoidably this approach causes him problems. For example, when he first learned about preorder, inorder and postorder traversals of trees, and was given code for a preorder print of a tree (shown on the left below), he simply cut and pasted the code, then moved the print statement to the correct location and renamed the procedure. However, he forgot to rename the procedure calls inside the code, resulting in the defective inorder print and postorder print code shown below.

```cpp
void prePrint(TNode t)
{
    output(t.value);
    if (t.left != null)
        prePrint(t.left);
    if (t.right != null)
        prePrint(t.right);
}
void inPrint(TNode t)
{
    if (t.left != null)
        prePrint(t.left);
    output(t.value);
    if (t.right != null)
        prePrint(t.right);
}
void postPrint(TNode t)
{
    if (t.left != null)
        prePrint(t.left);
    if (t.right != null)
        prePrint(t.right);
    output(t.value);
}
```

At this point, Anatoly did not behave like a typical student. He actually tested his code! Unfortunately, when the results were not correct, he reverted back to typical student behavior. He panicked and started randomly changing calls in all three procedures, hoping to get things right. Needless to say, the situation became even worse now than when he started.

Anatoly’s professor tested the code on a random tree of characters. When she looked at the output of his three print routines, she correctly guessed what had happened. However, instead of going directly to his code, she decided to try to reconstruct Anatoly’s code just by observing the output. In order to do this, she correctly made the following assumptions:

1. The output statement in each print routine is in the correct location (for example, between the two recursive calls in the inPrint routine).
2. Among the six recursive calls made by the three routines, exactly two calls are to prePrint, exactly two are to inPrint, and exactly two are to postPrint, though potentially in the wrong routines.

Soon the professor realized that reconstructing Anatoly’s code and the test tree from his output was not a simple task and that the result might be ambiguous. You will have to help her find all possible reconstructions of Anatoly’s code. In addition, for each such reconstruction, you are to find the alphabetically first tree (as described in the output section) giving the observed output.

## 输入格式
The input consists of a single test case. A test case consists of three strings on three separate lines: the observed output of Anatoly’s `prePrint`, `inPrint` and `postPrint` routines (in that order) on some test tree. Each of these strings consists of $n$ uppercase letters $(4 \leq n \leq 26)$, with no repeated letters in any string. The test case is guaranteed to have at least one solution.

## 输出格式
Display all possible reconstructions for the test case, ordered as described in the last paragraph below. The output for each reconstruction consists of two parts. The first part is a single line and describes the six calls in Anatoly’s routines: first the two (recursive) calls in Anatoly’s `prePrint` routine, followed by the calls in his `inPrint` routine, and finally the calls in his `postPrint` routine. The calls are described by the words `Pre`, `In`, and `Post`, separated by spaces. For example, if Anatoly’s routines were correct, the resulting output of the first part of the reconstruction would be `Pre Pre In In Post Post`.

The second part consists of three lines and describes the first test tree that could have generated the observed outputs. The first line is the *correct* preorder print of the tree, and the second and third lines contain the correct inorder and postorder prints, respectively. The first tree is the one with the alphabetically first preorder print. If there are multiple such trees, the first of these is the one with the alphabetically first inorder print.

Every reconstruction is a sequence of $6$ tokens chosen from `Pre`, `In`, and `Post`. The ordering of reconstructions is lexicographic with respect to the following ordering of tokens: Pre < In < Post.

## 题目大意
**【题目描述】**

Anatoly Cheng McDougal 在许多方面都是典型的学生。每当可能时，他都会尝试剪切和粘贴代码，而不是从头开始编写。不可避免地，这种方法给他带来了问题。例如，当他第一次学习树的前序、中序和后序遍历，并获得了前序打印树的代码（如下面左侧所示），他只是简单地剪切和粘贴代码，然后将打印语句移动到正确的位置并重命名过程。然而，他忘记了在代码内部重命名过程调用，导致了下面有缺陷的中序打印和后序打印代码。

```cpp
void prePrint(TNode t)
{
    output(t.value);
    if (t.left != null)
        prePrint(t.left);
    if (t.right != null)
        prePrint(t.right);
}
void inPrint(TNode t)
{
    if (t.left != null)
        prePrint(t.left);
    output(t.value);
    if (t.right != null)
        prePrint(t.right);
}
void postPrint(TNode t)
{
    if (t.left != null)
        prePrint(t.left);
    if (t.right != null)
        prePrint(t.right);
    output(t.value);
}
```

此时，Anatoly 不像典型的学生那样行事。他实际上测试了他的代码！不幸的是，当结果不正确时，他又恢复了典型的学生行为。他慌乱了，开始随机更改所有三个过程中的调用，希望能弄对。不用说，现在的情况比他刚开始时更糟糕了。

Anatoly 的教授在一个随机的字符树上测试了代码。当她查看他三个打印例程的输出时，她正确猜测到发生了什么。然而，她没有直接查看他的代码，而是决定仅通过观察输出来重建Anatoly的代码。为了做到这一点，她正确地做出了以下假设：

1. 每个打印例程中的输出语句在正确的位置（例如，在 `inPrint` 例程中的两个递归调用之间）。
2. 在三个例程中进行的六次递归调用中，恰好有两次调用 `prePrint`，两次调用 `inPrint` 和两次调用 `postPrint`，尽管它们可能在错误的例程中。

不久，教授意识到从Anatoly的输出重建代码和测试树并不是一件简单的任务，结果可能是模棱两可的。你需要帮助她找出所有可能的Anatoly代码重建方式。此外，对于每种重建方式，你需要找出字母顺序最早的树（如下面输出部分所描述的）。

**【输入格式】**

输入包含一个测试用例。一个测试用例由三行字符串组成：Anatoly 的 `prePrint`、`inPrint` 和 `postPrint` 例程在某个测试树上的观察输出（按顺序）。每个字符串由 $n$ 个大写字母组成（$4 \leq n \leq 26$），每个字符串中没有重复的字母。保证测试用例至少有一种解决方案。

**【输出格式】**

显示测试用例的所有可能重建方式，按照以下最后一段中描述的顺序排序。每种重建方式的输出分为两部分。第一部分是单行描述Anatoly例程中的六次调用：首先是Anatoly的 `prePrint` 例程中的两次（递归）调用，然后是 `inPrint` 例程中的调用，最后是 `postPrint` 例程中的调用。调用由单词 `Pre`、`In` 和 `Post` 描述，用空格分隔。例如，如果Anatoly的例程是正确的，则重建方式的第一部分的输出将是 `Pre Pre In In Post Post`。

第二部分包括三行，描述能够生成观察输出的第一棵树。第一行是树的正确前序遍历打印，第二行和第三行分别包含正确的中序遍历和后序遍历打印。第一棵树是按字母顺序最早的前序打印树。如果有多棵这样的树，则选择其中前序打印字母顺序最早的树。

每种重建方式都是从 `Pre`、`In` 和 `Post` 中选择的六个标记的序列。重建方式的排序是按照以下标记的词法顺序：`Pre` < `In` < `Post`。

翻译来自于：[ChatGPT](https://chatgpt.com/)


```input1
HFBIGEDCJA
BIGEDCJFAH
BIGEDCJFAH
```

```output1
Pre Post In Post In Pre
HFBJCDEGIA
BIGEDCJFAH
IGEDCJBAFH
```

```input2
BNLFAGHPEDOCMJIK
NLBGAPHCODEIJMKF
NLFAGHPEDOCMJIKB
```

```output2
In Pre In Post Post Pre
BLNFKMEHAGPCODIJ
NLBAGHPEODCMIJKF
NLGAPHDOCEJIMKFB
Post Pre In In Post Pre
BLNFKICPGAHEODMJ
NLBGAPHCODEIJMKF
NLAGHPDOECJMIKFB
```

