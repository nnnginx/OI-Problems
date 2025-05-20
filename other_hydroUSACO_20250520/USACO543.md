这个问题需要你写一个程序完成字符识别的任务。 每个完整的字符图案有 20 行，20 位。每个位是“0”或“1”。图 1a 对应着输入文件中的符号图案。 文件 font.in 包括了27个字符图案的信息，以这样的顺序记录： `_abcdefghijklmnopqrstuvwxyz` 其中 _ 表示空格字符。每个完整字符长 20 行。 输入文件包含一个或多个可能损坏的字符图案。一个字符图案可能以这些方式被损坏。 最多有一行被可能被复制了（就接在原来那一行的下面） 最多有一行可能丢失了 有些“0”可能被改成“1” 有些“1”可能被改成“0” 不会有任何一个字符图案既多余了一行并且又丢失了一行。在测试数据的任何一个字符图案中，“0”和“1”的被改变率不超过 30%。 被复制的那一行中，原来的行和多余的行可能都损坏了，而且损坏的部分可能并不相同。 写一个程序，使用 font.in 提供的字体，在输入文件提供的图象中识别出一个或多个的字符序列。 使用提供的字体图象来识别字符的时候，要找出最佳的多余行或遗漏行，使找出的所有“0”和“1”的变化数量最小。在所有可能的多余行中，只按损坏数据最少的那一行计算。你必须确定和输入序列最接近的字符序列（就是损坏数据最少的那一个）。每个测试数据有唯一的最优解。 正确的解答必须使用到输入文件中的所有数据。  
  
输入  
两个输入文件都以一个整数 N 开始（19 < N < 1200），表示接下去的行数。 N (位1)(位2)(位3) ... (位20) (位1)(位2)(位3) ... (位20) ... 每行有20位的宽度。在0和1之间没有空格分开。 文件 font.in 描述字体。它总有 541 行。它在每个测试数据中可能不同。  
  
输出  
你的程序必须建立一个输出文件，包含一个识别出来的字符串。它的格式是一个单行的 ASCII 文本。输出文件中不应该包含任何分隔符。如果你的程序没有识别出一个特定的字符，就必须在适当的位置输出一个“?”。  
  
## Description  
This problem requires you to write a program that performs character recognition.  
Each ideal character image has 20 lines of 20 digits. Each digit is a `0' or a `1'. See Figure 1a (way below) for the layout of character images in the file.  
The file font.in contains representations of 27 ideal character images in this order:  
`_abcdefghijklmnopqrstuvwxyz`  
where `_` represents the space character. Each ideal character is 20 lines long.  
The input file contains one or more potentially corrupted character images. A character image might be corrupted in these ways:  
  
- at most one line might be duplicated (and the duplicate immediately follows)  
- at most one line might be missing  
- some 0's might be changed to 1's  
- some 1's might be changed to 0's.  
- No character image will have both a duplicated line and a missing line. No more than 30% of the 0's and 1's will be changed in any character image in the evaluation datasets.  
  
In the case of a duplicated line, one or both of the resulting lines may have corruptions, and the corruptions may be different.  
Write a program to recognize the sequence of one or more characters in the image provided in the input file using the font provided in file font.in.  
Recognize a character image by choosing the font character images that require the smallest number of overall changed 1's and 0's to be corrupted to the given font image, given the most favourable assumptions about duplicated or omitted lines. Count corruptions in only the least corrupted line in the case of a duplicated line. You must determine the sequence of characters that most closely matches the input sequence (the one that requires the least number of corruptions). There is a unique best solution for each evaluation dataset.  
A correct solution will use precisely all of the data supplied in the input file.  
## INPUT FORMAT (both input files)  
Both input files begin with an integer N (19 <= N < 1200) that specifies the number of lines that follow:  
N  
(digit1)(digit2)(digit3) ... (digit20)  
(digit1)(digit2)(digit3) ... (digit20)  
...  
Each line of data is 20 digits wide. There are no spaces separating the zeros and ones.  
The file font.in describes the font. It will always contain 541 lines. It may differ for each evaluation dataset.  
## SAMPLE INPUT (file charrec.in)  
Incomplete sample showing the beginning of font.in(space and a)  
Sample charrec.in, showing an `a` corrupted  
  
font.in:  
  
```  
540  
00000000000000000000  
00000000000000000000  
00000000000000000000  
00000000000000000000  
00000000000000000000  
00000000000000000000  
00000000000000000000  
00000000000000000000  
00000000000000000000  
00000000000000000000  
00000000000000000000  
00000000000000000000  
00000000000000000000  
00000000000000000000  
00000000000000000000  
00000000000000000000  
00000000000000000000  
00000000000000000000  
00000000000000000000  
00000000000000000000  
00000000000000000000  
00000000000000000000  
00000000000000000000  
00000011100000000000  
00000111111011000000  
00001111111001100000  
00001110001100100000  
00001100001100010000  
00001100000100010000  
00000100000100010000  
00000010000000110000  
00000001000001110000  
00001111111111110000  
00001111111111110000  
00001111111111000000  
00001000000000000000  
00000000000000000000  
00000000000000000000  
00000000000000000000  
00000000000000000000  
```  
  
charrec.in:  
  
```  
19  
00000000000000000000  
00000000000000000000  
00000000000000000000  
00000011100000000000  
00100111011011000000  
00001111111001100000  
00001110001100100000  
00001100001100010000  
00001100000100010000  
00000100000100010000  
00000010000000110000  
00001111011111110000  
00001111111111110000  
00001111111111000000  
00001000010000000000  
00000000000000000000  
00000000000001000000  
00000000000000000000  
00000000000000000000  
```  
  
## OUTPUT FORMAT  
Your program must produce an output file that contains a single string of the characters recognized. Its format is a single line of ASCII text. The output should not contain any separator characters. If your program does not recognize a particular character, it must output a ? in the appropriate position.  
## SAMPLE OUTPUT  
a  
Note that the 'sample output' formerly displayed a blank followed by an 'a', but that seems wrong now.   