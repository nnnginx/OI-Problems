<p>Your task is to compute natural logarithm of the absolute value of the&nbsp;<a href="https://en.wikipedia.org/wiki/Bernoulli_number">Bernoulli number</a>&nbsp;for many integer parameters&nbsp;<strong>N</strong>.</p>
<p>I/O format is the same as in&nbsp;<a href="../BINARYIO/">BINARYIO</a>.</p>
<h3>Input</h3>
<p>Array of unsigned 32 bit integers in binary format (use <a href="http://www.cplusplus.com/reference/cstdio/fread/">fread</a>&nbsp;in C/C++)</p>
<p>To read <em>unsigned N</em> use <em>fread(&amp;N, sizeof(N), 1, stdin)</em>&nbsp; instead of usual <em>scanf("%u", &amp;N)</em> until the end of file.</p>
<p style="text-align: justify;">For each test case 2&nbsp;¡Ü&nbsp;<strong>N</strong>&nbsp;&lt; 2<sup>32</sup>, <strong>N </strong>is even.&nbsp;There will be up to 1,250,000 numbers in input file.</p>
<h3>Output</h3>
<p>Array of&nbsp;<a href="http://en.wikipedia.org/wiki/Double-precision_floating-point_format">doubles</a>&nbsp;in binary format (use <a href="http://www.cplusplus.com/reference/cstdio/fwrite/">fwrite</a>&nbsp;in C/C++)</p>
<p>To write <em>double a</em> use <em>fwrite(&amp;a, sizeof(a), 1, stdout)</em>&nbsp; instead of usual <em>printf("%lf\n", a)</em>.</p>
<p>For each <strong>N</strong>&nbsp;output ln(|B<sub>N</sub>|) with absolute or relative error less than 10<sup>-15</sup></p>
<h3>Example</h3>
<p><strong>Input:</strong></p>
<p>4</p>
<p>10</p>
<p>50</p>
<p><strong>Output:</strong></p>
<p>-3,4011973816621553754132366916069</p>
<p>-2,580216829592325170273661603119</p>
<p>57,277060811865704087099873424857</p>
<h4><strong>Sample input and output are readable for your convenience!!! </strong></h4>
<p>TL = 5 * My time</p>