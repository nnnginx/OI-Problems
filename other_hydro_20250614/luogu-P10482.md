## ��Ŀ����
In the game of Sudoku, you are given a large 9 �� 9 grid divided into smaller 3 �� 3 subgrids. For example,

![](https://cdn.luogu.com.cn/upload/image_hosting/acjiq3ud.png)

Given some of the numbers in the grid, your goal is to determine the remaining numbers such that the numbers 1 through 9 appear exactly once in (1) each of nine 3 �� 3 subgrids, (2) each of the nine rows, and (3) each of the nine columns.

## �����ʽ
The input test file will contain multiple cases. Each test case consists of a single line containing 81 characters, which represent the 81 squares of the Sudoku grid, given one row at a time. Each character is either a digit (from 1 to 9) or a period (used to indicate an unfilled square). You may assume that each puzzle in the input will have exactly one solution. The end-of-file is denoted by a single line containing the word ��end��.

## �����ʽ
For each test case, print a line representing the completed Sudoku puzzle.

## ��Ŀ����
**����Ŀ������**

��������Ϸ�У�����һ����� 9 �� 9 ���񣬷ֳ��˽�С�� 3 �� 3 ���������磬

![](https://cdn.luogu.com.cn/upload/image_hosting/acjiq3ud.png)

�ڸ��������е�һЩ���ֺ����Ŀ����ȷ��ʣ������֣�ʹ������ 1 �� 9 ǡ�ó���������λ�ã�(1) �Ÿ� 3 �� 3 �������е�ÿһ����(2) �����е�ÿһ�����Լ� (3) �����е�ÿһ����

**�������ʽ��**

��������ļ����������������ÿ�����԰�����һ����ɣ����а��� 81 ���ַ�����Щ�ַ�������������� 81 ���������и�����ÿ���ַ�������һ�����֣��� 1 �� 9����һ����㣨���ڱ�ʾδ���ķ��񣩡�����Լ��������е�ÿ�����ⶼ��Ψһ�⡣�ļ��Ľ�β��һ�а������ʡ�end����ʾ��

**�������ʽ��**

����ÿ�����԰�������ӡһ�б�ʾ��ɵ��������⡣

���������ڣ�[ChatGPT](https://chatgpt.com/)

```input1
.2738..1..1...6735.......293.5692.8...........6.1745.364.......9518...7..8..6534.
......52..8.4......3...9...5.1...6..2..7........3.....6...1..........7.4.......3.
end
```

```output1
527389416819426735436751829375692184194538267268174593643217958951843672782965341
416837529982465371735129468571298643293746185864351297647913852359682714128574936
```

