���������Ҫ��дһ����������ַ�ʶ������� ÿ���������ַ�ͼ���� 20 �У�20 λ��ÿ��λ�ǡ�0����1����ͼ 1a ��Ӧ�������ļ��еķ���ͼ���� �ļ� font.in ������27���ַ�ͼ������Ϣ����������˳���¼�� `_abcdefghijklmnopqrstuvwxyz` ���� _ ��ʾ�ո��ַ���ÿ�������ַ��� 20 �С� �����ļ�����һ�����������𻵵��ַ�ͼ����һ���ַ�ͼ����������Щ��ʽ���𻵡� �����һ�б����ܱ������ˣ��ͽ���ԭ����һ�е����棩 �����һ�п��ܶ�ʧ�� ��Щ��0�����ܱ��ĳɡ�1�� ��Щ��1�����ܱ��ĳɡ�0�� �������κ�һ���ַ�ͼ���ȶ�����һ�в����ֶ�ʧ��һ�С��ڲ������ݵ��κ�һ���ַ�ͼ���У���0���͡�1���ı��ı��ʲ����� 30%�� �����Ƶ���һ���У�ԭ�����кͶ�����п��ܶ����ˣ������𻵵Ĳ��ֿ��ܲ�����ͬ�� дһ������ʹ�� font.in �ṩ�����壬�������ļ��ṩ��ͼ����ʶ���һ���������ַ����С� ʹ���ṩ������ͼ����ʶ���ַ���ʱ��Ҫ�ҳ���ѵĶ����л���©�У�ʹ�ҳ������С�0���͡�1���ı仯������С�������п��ܵĶ������У�ֻ�����������ٵ���һ�м��㡣�����ȷ��������������ӽ����ַ����У��������������ٵ���һ������ÿ������������Ψһ�����Ž⡣ ��ȷ�Ľ�����ʹ�õ������ļ��е��������ݡ�  
  
����  
���������ļ�����һ������ N ��ʼ��19 < N < 1200������ʾ����ȥ�������� N (λ1)(λ2)(λ3) ... (λ20) (λ1)(λ2)(λ3) ... (λ20) ... ÿ����20λ�Ŀ�ȡ���0��1֮��û�пո�ֿ��� �ļ� font.in �������塣������ 541 �С�����ÿ�����������п��ܲ�ͬ��  
  
���  
��ĳ�����뽨��һ������ļ�������һ��ʶ��������ַ��������ĸ�ʽ��һ�����е� ASCII �ı�������ļ��в�Ӧ�ð����κηָ����������ĳ���û��ʶ���һ���ض����ַ����ͱ������ʵ���λ�����һ����?����  
  
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