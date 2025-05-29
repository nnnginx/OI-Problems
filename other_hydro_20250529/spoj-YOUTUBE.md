<p>N students are bored in computer class so they watch funny video clips on YouTube.</p>
<p>The site contains K popular clips, numbered 1 through N. When a video clip is watched, a list of similar video clips is displayed on the side.</p>
<p>Every student picks a video clip from the main page and starts watching it. After exactly one minute every student gets bored of his or her video clip, so he opens the <strong>first </strong>video clip from the list of similar clips on the side (even if he already watched that clip).</p>
<p>Write a program that determines for each student which video clip he will be watching <strong>during the M-th minute </strong>of the class.</p>
<h3>Input</h3>
<p>The first line contains three integers N, K and M (1 ¡Ü N, K ¡Ü 100 000) (1 &lt; M ¡Ü 1 000 000 000), the numbers of students, video clips and minutes.</p>
<p>The second line contains N integers, each between 1 and K, the indices of video clips the students start watching.</p>
<p>The third line contains K integers, each between 1 and K, the index of the first similar clip for each video clip.</p>
<h3>Output</h3>
<p>Output N integers, the indices of video clips that students will be watching during the M-th minute.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>4 5 2<br>1 2 4 3<br>5 5 1 2 3
<strong><br>Output:</strong>
5 5 2 1<br><strong><br><br>Input:</strong><br>2 6 5<br>1 6<br>2 3 4 1 4 5<br><strong><br>Output:</strong><br>1 2<br></pre>