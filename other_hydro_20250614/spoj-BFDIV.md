<p>Everyone knows that our human ancestors relied on extraterrestrial beings to teach them about science and technology. After helping us build pyramids and chart the stars, our alien mentors decided we needed some time to grow in isolation, so they took some dolphins and left to colonise another planet. Just before leaving, though, they gave us instructions on how to contact them in case of an emergency, such as global warming, nuclear holocaust, or a shortage of fish. The intergalactic telephone they designed consisted of a large golden box powered by alien arc technology. It was entrusted to the United Anarchist Alliance, but was lost when they went to war with the Unified Anarchist League after unsuccessful negotiations to decide which name was more logical for anarchists to call themselves. It remained lost for several centuries at the bottom of a lake until renowned archaeologists Indiana Serkis and Meronym Spader discovered it by chance during a fishing trip. Upon opening the box and pressing the large red button they found inside, an ancient alien immediately appeared and asked them deep, probing questions to determine whether humanity had advanced to the point where the aliens could come back to Earth and chill with us. Among other things, the aliens asked Indiana what his favorite color was, and what the result would be if 38157917385 were divided by 53387519, expressed as quotient and remainder. Since mathematics was never Indiana¡¯s or Meronym¡¯s strong suit, they¡¯ve asked you to write a program for them to perform such computations automatically. They have a computer with them that only understands one language, but they assure you that despite its simplicity the language is Turing complete and perfectly capable of computing the desired quantities efficiently.</p>
<p><strong>Note:</strong> You can use any programming language you want, as long as it is brainf**k.</p>
<h3>Input</h3>
<p>The first line contains an integer <strong>T</strong> (1 ¡Ü <strong>T</strong> ¡Ü 1000). Then follow <strong>T</strong> lines, each containing integers <strong>x</strong> (0 ¡Ü <strong>x</strong> ¡Ü 10^20) and <strong>y</strong> (1 ¡Ü <strong>y</strong> ¡Ü 10^20) separated by a single space. Each line, including the last, is terminated by a single newline (linefeed) character, which has ASCII value 10.</p>
<h3>Output</h3>
<p><strong>T</strong> lines containing the quotient and remainder of <strong>x</strong> divided by <strong>y</strong>, separated by a space.</p>
<h3>Example</h3>
<p><strong>Input:</strong></p>
<pre>5
0 42
42 42
123 45
12 345
10000 42
</pre>
<p><strong>Output:</strong></p>
<pre>0 0
1 0
2 33
0 12
238 4
</pre>
<h3>Additional Info</h3>
<p>There are two randomly generated data sets, one with <strong>T</strong>=1000 and the other with <strong>T</strong>=500. The average number of digits in <strong>x</strong> is about 13.5, the average number of digits in <strong>y</strong> is about 8, and the probability that the quotient is nonzero is about 0.82.</p>
<p>My solution at the time of publication has 1516 bytes (not golfed) and runs in 0.14s with 1.9M memory footprint.</p>