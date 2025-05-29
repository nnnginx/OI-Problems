<p style="box-sizing: border-box; margin: 0px 0px 10px; color: #3e3f3a; font-family: &quot;PT Sans&quot;; font-size: 14px; line-height: 20px;">Little Rumon is an enthusiast lad. One day while he was exploring the basement of their house for old garbage to find out any usable tool, he suddenly found an interesting device which had a display and a button. He found that if the button is pressed for t seconds, t random binary digits are displayed.</p>
<p style="box-sizing: border-box; margin: 0px 0px 10px; color: #3e3f3a; font-family: &quot;PT Sans&quot;; font-size: 14px; line-height: 20px;">It always had two property:-</p>
<p style="box-sizing: border-box; margin: 0px 0px 10px; color: #3e3f3a; font-family: &quot;PT Sans&quot;; font-size: 14px; line-height: 20px;">i) The binary number generated has no leading zeros.</p>
<p style="box-sizing: border-box; margin: 0px 0px 10px; color: #3e3f3a; font-family: &quot;PT Sans&quot;; font-size: 14px; line-height: 20px;">ii) There is no consecutive 1¡¯s in the number.</p>
<p style="box-sizing: border-box; margin: 0px 0px 10px; color: #3e3f3a; font-family: &quot;PT Sans&quot;; font-size: 14px; line-height: 20px;">Suppose, t = 4, then the possible outcomes are 1000, 1001, 1010.</p>
<p style="box-sizing: border-box; margin: 0px 0px 10px; color: #3e3f3a; font-family: &quot;PT Sans&quot;; font-size: 14px; line-height: 20px;">Rumon instantly rushed to his elder brother Shovon to show him what he had found. After testing the device, Shovon also got interested because the device was generating some number that is equal to the decimal representation of some Cricket South African player¡¯s jersey number.</p>
<p style="box-sizing: border-box; margin: 0px 0px 10px; color: #3e3f3a; font-family: &quot;PT Sans&quot;; font-size: 14px; line-height: 20px;">As for example, the device generated 1, 10001 and 1000 respectively which decimal representations are 1, 17 and 8, which are Hashim Amla, AB de Villiers and Dale Steyn¡¯s jersey numbers respectively.</p>
<p style="box-sizing: border-box; margin: 0px 0px 10px; color: #3e3f3a; font-family: &quot;PT Sans&quot;; font-size: 14px; line-height: 20px;">They started to call such numbers ¡°Binary Protean Number¡±.</p>
<p style="box-sizing: border-box; margin: 0px 0px 10px; color: #3e3f3a; font-family: &quot;PT Sans&quot;; font-size: 14px; line-height: 20px;">By the time, Rumon wondered if he writes down a binary protean number on a paper, what will be it¡¯s position in all possible binary protean number¡¯s sorted list.</p>
<p style="box-sizing: border-box; margin: 0px 0px 10px; color: #3e3f3a; font-family: &quot;PT Sans&quot;; font-size: 14px; line-height: 20px;">Shovon wanted to write a C program to answer Rumon¡¯s question, but then he thought that there is an upcoming Programming Contest arranged by ¡°Programming Problem in Bengali¡± Facebook group. So he decided to set it as a programming problem.</p>
<p style="box-sizing: border-box; margin: 0px 0px 10px; color: #3e3f3a; font-family: &quot;PT Sans&quot;; font-size: 14px; line-height: 20px;">Now it¡¯s your job to help little Rumon.</p>
<p style="box-sizing: border-box; margin: 0px 0px 10px; color: #3e3f3a; font-family: &quot;PT Sans&quot;; font-size: 14px; line-height: 20px;">Formally, given K¡¯th Binary Protean Number, you have to find the value of K.</p>
<h3>Input</h3>
<p><span style="color: #3e3f3a; font-family: &quot;PT Sans&quot;; font-size: 14px; line-height: 20px;">The first line of the input file contains an integer T. 1 &lt;=T &lt;= 75000. Then follows T cases. Every case consists of one line. The line contains a Binary Protean Number. It has no leading zeros and no consecutive ones in it. If the length of the Binary Protean Number is L then 1 &lt;= L &lt;= 90.</span></p>
<h3>Output</h3>
<p style="box-sizing: border-box; margin: 0px 0px 10px; color: #3e3f3a; font-family: &quot;PT Sans&quot;; font-size: 14px; line-height: 20px;">For every case, you should output a line containing the case number and the value of K. The output format is: Case X: K Where X is the case number. It is guaranteed that K will fit in 64 bit long long integer.</p>
<p style="box-sizing: border-box; margin: 0px 0px 10px; color: #3e3f3a; font-family: &quot;PT Sans&quot;; font-size: 14px; line-height: 20px;">See Sample input/output section for better understanding.</p>
<h3>Sample</h3>
<pre><strong>Input:</strong>
<span style="color: #3e3f3a; font-family: &quot;Ubuntu Mono&quot;; font-size: 14px; line-height: 20px;">3
1
100
1010</span></pre>
<pre><strong>Output:</strong>
<span style="color: #3e3f3a; font-family: &quot;Ubuntu Mono&quot;; font-size: 14px; line-height: 20px;">Case 1: 1
Case 2: 3
Case 3: 7</span></pre>