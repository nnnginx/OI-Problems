<p>Veronica attends a music academy. She was given a music sheet of a composition with only notes (without annotations), and needs to recognise the scale used. In this problem, we will limit ourselves to only the two most frequently used (and usually taught in schools first) scales: A-minor and C-major. This doesn't make them simpler or more basic than other minor and major scales ¨C all minor scales are mutually equivalent save for translation, and so are major scales.</p>
<p>Still, out of the 12 tones of an octave {A, A#, B, C, C#, D, D#, E, F, F#, G, G#} used in modern music, A-minor and C-major scales do use the tones with shortest names: A-minor is defined as an ordered septuple (A, B, C, D, E, F, G), and C-major as (C, D, E, F, G, A, B).</p>
<p>Notice that the sets of tones of these two scales are equal. What's the difference? The catch is that not only the set of tones, but also their usage, determines a scale. Specifically, the <strong>tonic</strong> (the first tone of a scale), <strong>subdominant</strong> (the fourth tone) and <strong>dominant</strong> (the fifth tone) are the primary candidates for accented tones in a composition. In A-minor, these are A, D, and E, and in C-major, they are C, F, and G. We will name these tones <strong>main tones</strong>.</p>
<p>Aren't the scales still equivalent save for translation? They are not: for example, the third tone of A- minor (C) is three half-tones higher than the tonic (A), while the third tone of C-major (E) is four half- tones higher than the tonic (C). The difference, therefore, lies in the intervals. This makes minor scales ¡°sad¡± and major scales ¡°happy¡±.</p>
<p>Write a program to decide if a composition is more likely written in A-minor or C-major by counting whether there are more <strong>main tones</strong> of A-minor or of C-major among the <strong>accented</strong> tones (<strong>the first tones in each measure</strong>). If there is an <strong>equal</strong> number of main tones, determine the scale based on the <strong>last tone</strong> (which is guaranteed to be either A for A-minor or C for C-major in any such test case).</p>
<p>For example, examine the well-known melody ¡°Fr¨¨re Jacques¡±:</p>
<p style="text-align: center;">CD|EC|CD|EC|EF|G|EF|G|GAGF|EC|GAGF|EC|CG|C|CG|C</p>
<p>The character ¡°|¡± separates measures, so the accented tones are, in order: C, E, C, E, E, G, E, G, G, E, G, E, C, C, C, C. Ten of them (C, C, G, G, G, G, C, C, C, C) are main tones of C-major, while six (E, E, E, E, E, E) are main tones of A-minor. Therefore, our best estimate is that the song was written in C-major.</p>
<h3>Input</h3>
<p>The first and only line of input contains a sequence of at least 5, and at most 100, characters from the set {¡°A¡±, ¡°B¡±, ¡°C¡±, ¡°D¡±, ¡°E¡±, ¡°F¡±, ¡°G¡±, ¡°|¡±}. This is a simplified notation for a composition, where the character ¡°|¡± separates measures. The characters ¡°|¡± will never appear adjacent to one another, at the beginning, or at the end of the sequence.</p>
<h3>Output</h3>
<p>The first and only line of output must contain the text ¡°C-dur¡± (for C-major) or ¡°A-mol¡± (for A- minor).</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
AEB|C

<strong>Output:</strong>
C-dur
</pre>
<pre><strong>Input:</strong>
CD|EC|CD|EC|EF|G|EF|G|GAGF|EC|GAGF|EC|CG|C|CG|C

<strong>Output:</strong>
C-dur
</pre>