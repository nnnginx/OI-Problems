<!-- 		@page { margin: 2cm } 		P { margin-bottom: 0.21cm } -->
<p><strong><span style="color: #008000;">(the english version is following the spanish version at each section, and is in green letters)</span></strong></p>
<p><span style="font-size: small;"><span style="font-family: Verdana,sans-serif;">Una secuencia de <em>k </em>n¨²meros enteros positivos <em>, (k &gt; 1), </em>es <strong>saltarina</strong><span style="font-weight: normal;">,</span> si los valores absolutos de las diferencias entre elementos sucesivos toman todos los valores posibles desde 1 hasta <em>k-1.</em></span></span></p>
<p style="font-style: normal;"><span style="font-size: small;"><span style="font-family: Verdana,sans-serif;">Por ejemplo: la secuencia 51423, es una secuencia saltarina de longitud 5, porque las diferencias entre los elementos sucesivos de la secuencia son: 4,3,2,1</span></span></p>
<p><span style="font-size: small;"><span style="font-family: Verdana,sans-serif;">Se desea conocer cu¨¢ntas secuencias saltarinas hay de longitud L.</span></span></p>
<p><span style="font-size: small;"><span style="font-family: Verdana,sans-serif;">En este problema consideramos que las secuencias est¨¢n formadas ¨²nicamente por valores en 1..k.</span></span></p>
<!-- 		@page { margin: 2cm } 		P { margin-bottom: 0.21cm } -->
<p style="margin-bottom: 0cm;"><span style="font-family: verdana,geneva;"><span style="color: #008000;">A</span><span style="color: #008000;"><span style="font-size: small;"><span style="color: #008000;"> seq</span>uence of <em>k &gt; 1</em> integers is called a <em>jolly jumper</em> if the absolute values of the difference between successive elements take on all the values 1 through <em>k-1</em>.  For instance, </span></span></span></p>
<p style="margin-bottom: 0cm;"><span style="font-family: verdana,geneva;"><span style="color: #008000;"><span style="font-size: small;">the sequence 51423 is a jolly jumper of lenght 5, because the differences between consecutive elements are 4,3,2,1</span></span></span></p>
<p style="margin-bottom: 0cm;"><span style="font-family: verdana,geneva;"><span style="color: #008000;"><span style="font-size: small;">You must to find out how many jolly jumpers are with lenght = L.</span></span></span></p>
<p style="margin-bottom: 0cm;"><span style="font-family: verdana,geneva;"><span style="color: #008000;"><span style="font-size: small;">(in this problem we only consider the jolly jumpers built with values only in the 1..k range).<br></span></span></span></p>
<p>&nbsp;</p>
<p style="margin-bottom: 0cm;"><strong><span style="font-family: Verdana,sans-serif;"><span style="font-size: medium;">Input</span></span></strong></p>
<p style="margin-bottom: 0.5cm;"><span style="font-size: small;"><span style="font-family: Verdana,sans-serif;">Cada l¨ªnea de la entrada consta de un entero k, (&gt; 1). Cada l¨ªnea es un caso diferente para informar. La entrada termina con una l¨ªnea conteniendo el valor 0, el cual no se procesa.</span></span></p>
<p style="margin-bottom: 0cm;"><span style="font-family: verdana,geneva;"><span style="color: #008000;"><span style="font-size: small;">Each line of the input have an integer k, (&gt; 1). Each line is a different case to process. The input ends with a line that contains the value 0 (this value is the end of data signal and won't be processed).</span></span></span></p>
<p style="margin-bottom: 0cm;"><strong><span style="font-family: Verdana,sans-serif;"><span style="font-size: medium;">Output</span></span></strong></p>
<p style="margin-bottom: 0.5cm;"><span style="font-size: small;"><span style="font-family: Verdana,sans-serif;">Por cada l¨ªnea de la entrada, se debe generar una l¨ªnea de salida que informa la cantidad de secuencias saltarinas de longitud igual a k.</span></span></p>
<p style="margin-bottom: 0cm;"><span style="font-family: verdana,geneva;"><span style="color: #008000;"><span style="font-size: small;">Your program must to generate one output line for each input line. At each output line you must inform the quantity of jolly jumpers with length equal to k.</span></span></span></p>
<p style="margin-bottom: 0cm;"><strong><span style="font-family: Verdana,sans-serif;"><span style="font-size: medium;">Sample Input</span></span></strong></p>
<p><span style="font-size: small;">2</span></p>
<p><span style="font-size: small;">3</span></p>
<p><span style="font-size: small;">4</span></p>
<p><span style="font-size: small;">0</span></p>
<pre><br></pre>
<p style="margin-bottom: 0cm;">&nbsp;</p>
<p style="margin-bottom: 0cm;"><strong><span style="font-family: Verdana,sans-serif;"><span style="font-size: medium;">Sample Output</span></span></strong></p>
<p><span style="font-size: small;">2</span></p>
<p><span style="font-size: small;">4</span></p>
<p><span style="font-size: small;">4</span></p>
<pre><br><br></pre>
<p style="margin-bottom: 0cm;">&nbsp;</p>