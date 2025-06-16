<p><strong>(EN:)</strong></p>
<p>Every tourist visiting our city must visit the May 4 avenue. There are <strong>N</strong> houses, numbered from 1 to <strong>N</strong>. There are <strong>P</strong><sub>i</sub> people living at house <em>i</em>.</p>
<p>The statistic institute is procedding with the survey this year. They will make many queries about the avenue's population. For each query, two numbers <strong>A </strong>and <strong>B</strong>, with <strong>A</strong> &lt;= <strong>B</strong>, are given. You must determine the total number of people living in all houses from house <strong>A</strong> to house <strong>B</strong>, inclusive.</p>
<h3>Input</h3>
<p>First line contains the number&nbsp; <strong>N</strong> (1 &lt;= <strong>N</strong> &lt;= 10<sup>5</sup>). Second line contains <strong>N</strong> integers <strong>P</strong><sub>1</sub>, <strong>P</strong><sub>2</sub>, ..., <strong>P</strong><sub>N</sub>, indicating how many people live at each house (for each 1 &lt;= i &lt;= <strong>N</strong>, 0 &lt;= <strong>P</strong><sub>i</sub> &lt;= 100). Next line contains the integer <strong>Q</strong> (1 &lt;= <strong>Q</strong> &lt;= 10<sup>4</sup>), the number of queries to be processed. Each of the next <strong>Q</strong> lines describes a query with two integers <strong>A</strong> and <strong>B</strong> (1 &lt;= <strong>A</strong> &lt;= <strong>B</strong> &lt;= <strong>N</strong>).</p>
<h3>Output</h3>
<p>For each query, print a line with its result.</p>
<p><strong>(PT-BR:)</strong></p>
<p>Todo turista que visita a cidade deve conhecer a Avenida Quatro de Maio. Há <strong>N</strong> casas na avenida, numeradas sequencialmente de 1 a <strong>N</strong>. Há <strong>P</strong><sub>i</sub> pessoas morando na casa de número <em>i</em> da avenida.<br><br>O instituto de estatística está realizando o censo deste ano. Para tal, o instituto irá realizar diversas consultas sobre a população da avenida. Em cada consulta, são dados dois números <strong>A</strong> e <strong>B</strong>, com <strong>A</strong> &lt;= <strong>B</strong>. Para cada consulta, é necessário determinar o número total de pessoas que moram entre as casas <strong>A</strong> e <strong>B</strong>, inclusive.<br><br>Sua tarefa é, dada a população de cada casa e as consultas que o instituto irá fazer, determinar a resposta para cada consulta dada.</p>
<h3>Entrada</h3>
<p>A primeira linha da entrada contém o inteiro <strong>N</strong> (1 &lt;= <strong>N</strong> &lt;= 10<sup>5</sup>). A segunda linha contém <strong>N</strong> inteiros <strong>P</strong><sub>1</sub>, <strong>P</strong><sub>2</sub>, ..., <strong>P</strong><sub>N</sub>, indicando a população de cada casa da avenida (Para cada 1 &lt;= i &lt;= <strong>N</strong>, 0 &lt;= <strong>P</strong><sub>i</sub> &lt;= 100). A terceira linha contém um inteiro <strong>Q</strong> (1 &lt;= <strong>Q</strong> &lt;= 10<sup>4</sup>), indicando o número de consultas a serem realizadas. Por fim, cada uma das próximas <strong>Q</strong> linhas descreve uma consulta. Cada linha contém dois inteiros <strong>A</strong> e <strong>B</strong> (1 &lt;= <strong>A</strong> &lt;= <strong>B</strong> &lt;= <strong>N</strong>).</p>
<h3>Saida</h3>
<p>Para cada consulta, imprima uma linha contendo sua resposta.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
4<br>10 2 8 72<br>3<br>4 4<br>1 3<br>2 4

<strong>Output:</strong>
72<br>20<br>82<br><br></pre>
<pre><strong>Input:</strong>
5<br>1 2 3 4 5<br>2<br>1 5<br>1 1

<strong>Output:</strong>
15<br>1<br><br><br></pre>