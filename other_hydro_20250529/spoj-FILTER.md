<p>The median filter is a nonlinear digital filter used to reduce noise in images, sounds, and other kinds of signals.
It examines each sample of the input through a <i>window</i> and then emits the <i>median</i> of the samples in the window.
Roughly speaking, a window is an interval that contains a target sample and its preceding and succeeding
samples; the median of a series of values is given by the middle value of the series arranged in ascending (or
descending) order.</p>
<p>Let us focus on a typical median filter for black-and-white raster images. The typical filter uses a 3 ¡Á 3 window,
which contains a target pixel and the eight adjacent pixels. The filter examines each pixel in turn through this
3 ¡Á 3 window, and outputs the median of the nine pixel values, i.e. the fifth lowest (or highest) pixel value, to the
corresponding pixel. We should note that the output is just given by the pixel value in majority for black-andwhite
images, since there are only two possible pixel values (i.e. black and white). The figure below illustrates
how the filter works.</p>
<center><img src="/content/crazyb0y:FILTER_A.jpg"></center>
<p>The edges of images need to be specially processed due to lack of the adjacent pixels. In this problem, we extends
the original images by repeating pixels on the edges as shown in the figure below. In other words, the lacked
pixels take the same values as the nearest available pixels in the original images.</p>
<center><img src="/content/crazyb0y:FILTER_B.jpg"></center>
<p>You are requested to write a program that reads images to which the filter is applied, then finds the original
images containing the greatest and smallest number of black pixels among all possible ones, and reports the
difference in the numbers of black pixels.</p>

<h3>Input</h3>

<p>The input contains a series of test cases.</p>
<p>The first line of each test case contains two integers W and H (1 ¡Ü W, H ¡Ü 8), which indicates the width and
height of the image respectively. Then H lines follow to describe the filtered image. The <i>i</i>-th line represents
the <i>i</i>-th scan line and contains exactly W characters, each of which is either '#' (representing black) or '.'
(representing white).</p>
<p>The input is terminated by a line with two zeros.</p>

<h3>Output</h3>

<p>For each test case, print a line that contains the case number followed by the difference of black pixels. If there
are no original images possible for the given filtered image, print "<tt>Impossible</tt>" instead.</p>
<p>Obey the format as shown in the sample output.</p>

<h3>Example</h3>
<pre><b>Input:</b>
5 5
#####
#####
#####
#####
#####
4 4
####
####
####
####
4 4
#...
....
....
...#
4 4
.#.#
#.#.
.#.#
#.#.
0 0

<b>Output:</b>
Case 1: 10
Case 2: 6
Case 3: 2
Case 4: Impossible
</pre>