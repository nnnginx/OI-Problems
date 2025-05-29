<p>On the gentle plains of Bytelandia, the mysterious ruffalo wander in herds solving combinatorics problems and searching for their next meals. Finding suitable food is becoming more and more difficult, as over the years the ruffalo have developed a curious diet consisting solely of permutations. To make matters worse, roughly half of all existing ruffalo lack the enzyme that would allow their stomachs to decompose permutations into cycles, and the other half are allergic to explicitly written fixed points.</p>

<p>The two great ruffalo leaders, Wildthings and Nowyouseemee, have joined forces to build a device that can automatically transform permutations into a notation that everyone can digest and enjoy (but not necessarily in that order). The bright young programmer Zodiac was assigned the task of building the device, but in a tragic freak accident he swallowed a fixed point and died shortly thereafter. Zodiac's assistants found a single sheet of paper lying next to his body on the laboratory floor with just eight symbols written on it: "+-&lt;&gt;[],.". Out of respect for Zodiac's dying wish, the Ruffalo High Council passed a decree that the device must be built entirely in branf**k, no matter what the cost. Nowyouseemee has personally offered an unprecedented reward of 54 Gifts of Heaven to anyone who can successfully complete the task. While nobody has ever seen a Gift of Heaven, it is said that they come in magical bright green boxes that become a little faded after a day, and a little more faded after a week.</p>

<p><strong>Note:</strong> You can use any programming language you want, as long as it is brainf**k. If you would like to submit in other languages, please see the <a href="http://www.spoj.com/problems/PERMCYC/">tutorial</a> version.</p>

<h3>Input</h3>

<p>The first line contains an integer <strong>T</strong> (1 �� <strong>T</strong> �� 5000). Then follow 2<strong>T</strong> lines, representing <strong>T</strong> test cases. The first line of each test case contains an integer <strong>N</strong> (1 �� <strong>N</strong> �� 9), and the second line contains a permutation of [1..<strong>N</strong>] as a space-separated list of <strong>N</strong> integers. Every line ends with a single newline character (ASCII 10), including the last line.</p>

<h3>Output</h3>

<p><strong>T</strong> lines containing the disjoint cycle decomposition of the corresponding permutation. For the identity permutation, print "e" without quotes. If there is more than one correct answer, print any of them.</p>

<h3>Example</h3>

<p><strong>Input:</strong></p>
<pre>5
3
1 2 3
3
2 1 3
4
2 1 4 3
9
3 8 9 4 1 7 6 2 5
9
3 8 9 4 1 7 6 2 5
</pre>

<p><strong>Output:</strong></p>
<pre>e
(1 2)
(1 2)(3 4)
(1 3 9 5)(2 8)(6 7)
(2 8)(9 5 1 3)(7 6)
</pre>

<h3>Additional Info</h3>

<p>There are two randomly generated data sets, one with <strong>T</strong>=5000 and the other with <strong>T</strong>=500. The average value of <strong>N</strong> in each data set is approximately 6.36.</p>

<p>The custom judge reports your source code length in parentheses after the judge result (when available at the time of judge termination). Only valid BF commands are counted. Also, if you don't get AC, you will be told on which data set you first failed (0-indexed). Thanks to <a href="http://www.spoj.com/users/tjandra/">(Tjandra Satria Gunawan)(������)</a> and <a href="http://www.spoj.com/users/crazyb0y/">Bin Jin</a>, who wrote judges using the same or similar ideas. The master judge C++ source code is available <a href="http://www.spoj.com/content/cyclops:bfprmcyc_master_judge">here</a>, and assumes that the test case judge reports source length as score.</p>

<p>For assessing the correctness of program output, the custom judge works just the same as the standard "Ignores extra whitespaces" judge, except that it allows any valid cycle decomposition. In case you don't understand how the standard judge works, this means that e.g. "( 1 2)" and "(1 2) (3 4)" would be judged as wrong for the second and third example cases respectively, but printing ten spaces instead of the single space in "(1 2)" is perfectly fine.</p>

<p>My solution at the time of publication has 334 bytes (golfed) and runs in 0.47s with 1.6M memory footprint.</p>

<p>Update: Reduced source to <a href="http://www.spoj.com/content/cyclops:bfprmcyc_submissions.png">292</a> as of 2014-04-30.</p>