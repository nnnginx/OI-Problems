<p><span style="font-size: x-large;"><strong>Laser Beam 2.0</strong></span></p>
<p><img src="../../../content/tjandra:D_cover.png" alt=""></p>
<p>Laser is a beam of light that can bounce if it hit a mirror, Satria who love beauty of nature make an experiment with grid of mirror and some laser, this is the second time Satria playing with laser, so he named his experiment "Laser Beam 2.0". The experiment is so great, many people like with Satria's experiment because that bouncing laser can make a beautiful pattern.</p>
<p>Gunawan who curious about beautiful pattern secretly experimenting with Satria's laser and mirror when Satria not home, but something terible happen, he accidentally crossed two different charged laser, so it break all the mirror and destroying Satria's experiment.</p>
<p>Fortunately, the blueprint of Satria's laser input/output is intact, but the blueprint of how the mirror is placed is burned so it's unreadable. Satria is sad, he should build the experiment from the beginning.</p>
<p>Tjandra who hear the tragedy come to Satria's house and know the condition. He suggest that no need for Satria to experiment from the beginning because the blueprint of Satria's laser input is intact.</p>
<p><span style="text-decoration: underline;">Satria said</span>: "Is it possible to recover my experimet? The mirror blueprint is gone, even if we have the laser input/output, we don't know how to dirrect the input laser to output laser"<br><span style="text-decoration: underline;">Tjandra replied</span>: "Maybe that's not true, it depend on how your blueprint is designed can I know more about your experiment and your blueprint?"<br><span style="text-decoration: underline;">Satria replied</span>: "<em>My experiment consiting of 2D grid of mirror and an array of lasers on each side (there are 4 sides) and each laser is shoot to inside of the grid, there are two kind of mirror, diagonal up '/' and diagonal down '\', based on my observation, diagonal up '/' mirror will bounce the laser with this rule: {from left to up; from up to left; from right to down; and from down to right}, and diagonal down '\' mirror will bounce the laser with this rule: {from left to down; from down to left; from right to up; and from up to right}. The blueprint tells about how laser are connected, after bouncing so many times, eventually the laser will go outside the grid and hit another laser, in that phenomena I call that two laser is 'connected'. In the blueprint each number appear exactly 2 times that's mean the laser with the same number are 'connected' each other.</em> That's my experiment and how the input/output blueprint work. So, is it possible using input/output blueprint to re-create missing mirror blueprint?"<br><span style="text-decoration: underline;">Tjandra replied</span>: "Yes, it's possible, but the result will probably be not the same as the old one because the mirror blueprint that satisfy your input/output blueprint is not unique"<br><span style="text-decoration: underline;">Satria replied</span>: "That's okay, if it satisfy the input/output blueprint, It'll always be as beautiful as original one"<br><span style="text-decoration: underline;">Tjandra replied</span>: "I'm glad to hear that. Okay, I know someone who is genious in programming, I'll call him to help you recover your experiment"</p>
<p>Now Tjandra call you using his old phone for help, because he believe that you're so promising to recover Satria's experiment. Can you help them?</p>
<p><span style="font-size: large;"><strong>Input</strong></span></p>
<p>The first line there are two integers X and Y denoting number of rows and number of colums respectively of Satria's mirror grid.<br>On the second line there are Y integers denoting array of laser on top of that grid that is initially shoot in down direction.<br>Each of next X lines there are two integers A<sub>i</sub> and B<sub>i</sub>:</p>
<ul>
<li>A<sub>i</sub> means i-th laser (counting from top to bottom) on left of that grid that is initially shoot in right direction.</li>
<li>B<sub>i</sub> means i-th laser (counting from top to bottom) on right of that grid that is initially shoot in left direction.</li>
</ul>
<p>The last line there are Y integers denoting array of laser on bottom of that grid that is initially shoot in up direction.</p>
<p><strong><span style="font-size: large;">Output</span></strong></p>
<p>If it's impossible to re-create Satria's mirror blueprint, print "-1" without the quotes.</p>
<p>Otherwise print X rows and Y collums of mirror blueprint, character '\' ASCII(92) denoting diagonal down mirror, and character '/' denoting diagonal up mirror.</p>
<p><strong><span style="font-size: large;">Constraint</span></strong></p>
<p>1 ¡Ü&nbsp;X ¡Ü&nbsp;100</p>
<p>1 ¡Ü&nbsp;Y ¡Ü 100</p>
<p>1 ¡Ü Each numbers that appears in the input (except X and Y) ¡Ü&nbsp;X+Y</p>
<p>Each numbers in the input (except X and Y) will appear excactly twice.</p>
<p><strong><span style="font-size: large;">Sample 1</span></strong></p>
<p><span style="text-decoration: underline;">Input</span></p>
<pre>1 1<br>1<br>1 2<br>2</pre>
<p><span style="text-decoration: underline;">Output</span></p>
<pre>/</pre>
<p><strong><span style="font-size: large;">Sample 2</span></strong></p>
<p><span style="text-decoration: underline;">Input</span></p>
<pre>1 1<br>1<br>2 1<br>2</pre>
<p><span style="text-decoration: underline;">Output</span></p>
<pre>\</pre>
<p><strong><span style="font-size: large;">Sample 3</span></strong></p>
<p><span style="text-decoration: underline;">Input</span></p>
<pre>3 1<br>1<br>1 3<br>2 2<br>3 4<br>4</pre>
<p><span style="text-decoration: underline;">Output</span></p>
<pre>-1</pre>
<p><strong><span style="font-size: large;">Sample 4</span></strong></p>
<p><span style="text-decoration: underline;">Input</span></p>
<pre>3 1<br>1<br>1 2<br>3 2<br>3 4<br>4</pre>
<p><span style="text-decoration: underline;">Output</span></p>
<pre>/<br>\<br>/</pre>
<p><strong><span style="font-size: large;">Sample 5</span></strong></p>
<p><span style="text-decoration: underline;">Input</span></p>
<pre>4 7<br>7 7 8 9 10 10 2<br>1 2<br>1 3<br>4 3<br>5 6<br>5 4 8 9 11 11 6</pre>
<p><span style="text-decoration: underline;">Output</span></p>
<pre>\/\\\/\<br>////\//<br>/\\\\\\<br>/////\/</pre>
<p><strong><span style="font-size: large;">Sample 5 Explanation</span></strong></p>
<p>If all pair of identical number on input is connected, then it'll satisfy Satria's input/output blueprint. Here is an image that show the correctness of sample 5 output.</p>
<p><img src="../../../content/tjandra:sample5.png" alt=""></p>