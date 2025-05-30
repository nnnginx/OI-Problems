<p>
Hugh F. Oh, in his never-ending quest to prove the existence of extraterrestrials, has gotten hold of
a number of nighttime photographs taken by a research group that is examining glowing swamp gas.
Hugh wants to see if any of the photos show, not swamp gas, but Little Grey Men in glowing suits. The
photographs consist of bright dots appearing against a black background. Unfortunately, at the time
the photos were taken, trains were travelling through the area (there is a train trestle over the swamp),
and occasional lights from the train windows also appear in the photographs. Hugh, being a fastidious
researcher, wants to eliminate these spots from the images. He can��t tell from the photos exactly where
the tracks are, or from what direction the photos were taken, but he knows that the tracks in that
area are perfectly straight, so he��s decided on the following approach: he will find the line with the
maximum number of spots lying on it and, if there are four or more spots on the line, he will eliminate
those points from his calculations, assuming that those are windows on the train. If two or more lines
have the maximum number of points, Hugh will just randomly select one such set and delete it from
the photo (he��s not all that fastidious �C after all, he believes in Little Grey Men). If there are fewer
than four points lying along a common line, Hugh will assume that there is no train in the photograph
and won��t delete any points. Please write a program for him to process a set of photographs.

</p><h3>Input</h3>
<p>
There will be a series of test cases. Each test case is one photograph described by a line containing
a positive integer n (&lt;= 1000) the number of distinct spots in the photograph, followed by n lines
containing the integer coordinates of the spots, one (x, y) pair per line. All coordinates are between 0
and 10000. The last photo description is followed by a line containing a zero, marking the end of the
input. This line should not be processed.

</p><h3>Output</h3>
<p>
For each test case, output the photo number followed by the number of points eliminated from the
photograph. Imitate the sample output below.


</p><h3>Example</h3>

<pre><b>Input:</b>
6
0 1
0 2
1 2
2 2
4 5
5 6
4
3 5
4 4
6 5
7 4
0

<b>Output:</b>
Photo 1: 4 points eliminated
Photo 2: 0 points eliminated
</pre>