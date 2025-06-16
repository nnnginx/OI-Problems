<p>Adorsho Ingreji Uccho Biddaloy has recently opened Media Studies department. Even though the name of the institute implies otherwise, it offers various courses on Bangla media too. As part of a course called Deshi Movie Analysis, the students of this department has to watch at least <strong>M</strong> minutes of movies that are being shown at various cinema halls across the city and submit their analysis report.</p>
<p>Nadim, a student of this department, thought it would be great at first. How many students get to watch movies for education, right? Wrong! He quickly found out how gravely mistaken he was seeing movie titles like ¡°Toke Valobashtei Hobe¡± and ¡°Matha Noshto¡±. He decides to do away with this task as fast as possible.</p>
<p>There are <strong>N</strong> cinema halls situated in a straight line (he lives in one of the most well planned cities in the world) one after another, each showing a defferent movie. His plan is to, given the length of each movie in minutes, select the least number of movies that will satisfy the M minutes of movie-watching requirement of the course. As he is lazy, he does not want to watch a movie in a hall and then go to a hall far away from the previous one to watch another movie. So, he decides to watch movies in halls so that the hall of a movie is situated next to the hall of the previous movie that he watched, if he watches multiple movies. A person can watch only one movie and only once at a hall any time he wishes. Once a person enters a hall, he cannnot leave before finishing the movie.</p>
<p>As stated before, he is lazy and has asked you, his best friend, to help him. You are lazy too, but you are a good programmer. So you decide to write a program.</p>
<h3>Input</h3>
<p>Input begins with a line containing a single integer <strong>T(1&lt;=T&lt;=100)</strong>, denoting the number of test cases. <strong>T</strong> test cases follow. Each test case begins with a line containing two integers <strong>N(1&lt;=N&lt;=10000)</strong> and <strong>M(0&lt;=M&lt;=10^9)</strong>, denoting the number of cinema halls(and thus the number of movies) and the minimum movie-watching experience required by the course respectively. The next line contains N space separated positive integers denoting the length of movies in minutes shown in cinema halls from left to right. These integers will not exceed 10^5.</p>
<h3>Output</h3>
<p>For each test case, output a single line in the format <strong>Case X: Y</strong>, where <strong>X</strong> denotes the test case number and <strong>Y</strong> denotes the minimum number of movies Nadim has to watch in consecutive cinema halls so that he earns at least M minutes of movie-watching experience. If he cannot complete this task, Y should be <strong>-1</strong>.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
10 15
5 1 3 5 10 7 4 9 2 8
5 11
1 2 3 4 5

<strong>Output:</strong>
Case 1: 2
Case 2: 3
</pre>