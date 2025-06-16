<p>In the set cover problem there is a collection <i>C =
{S<sub>1</sub>, ...,S<sub>m</sub>}</i> of subsets of the universe [<i>n</i>] = <i>{0, ...,n-1}</i>,
and one must
find a minimum-sized subcollection of <i>C</i> that still covers
[<i>n</i>] (it may be the case that <i>S<sub>i</sub></i> and <i>S<sub>j</sub></i> contain the exact same
elements for some <i>i</i> ¡Ù <i>j</i>).  A <b>path of length r</b> is a graph on
<i>r+1</i> vertices <i>v<sub>0</sub>, ...,v<sub>r</sub></i> where <i>v<sub>i</sub></i> has an undirected edge
to <i>v<sub>i+1</sub></i> for <i>i = 0, ...,r-1</i> (these are the only edges).
A set cover instance <i>I</i> is
said to be <b>path-realizable</b> if there exists a mapping from <i>I</i> to a
path of length <i>m</i> where the <i>S<sub>i</sub></i> are mapped to edges in the path
and each <i>i</i> in [<i>n</i>] is mapped to a pair of (not-necessarily distinct)
vertices <i>s<sub>i</sub></i>, <i>t<sub>i</sub></i> on the path such that the edges lying between
<i>s<sub>i</sub></i> and <i>t<sub>i</sub></i> correspond exactly to the sets of <i>C</i> that
contain <i>i</i>.  Two sets <i>S<sub>i</sub>,S<sub>j</sub></i> must be mapped to different edges on
the path if <i>i</i> ¡Ù <i>j</i>.  You will be given a set cover instance that is
guaranteed to be path-realizable and should output the size of a
minimum-sized subcollection of <i>C</i> still covering [<i>n</i>].

</p><h3>Input</h3>
<p>The first line of the input is "<i>N M</i>" (<i>1</i> ¡Ü N, M ¡Ü 300),
where <i>N</i> is the size of the universe and <i>M</i> is the number of sets
<i>S<sub>i</sub></i> in the collection of subsets of <i>{0, ...,N - 1}</i>.  What follows
are <i>M</i> groups of lines.  The <i>i</i>th group starts with one line
containing |<i>S<sub>i</sub></i>|, the size of the <i>i</i>th subset.  If |<i>S<sub>i</sub></i>| = <i>0</i>, the
current group of lines ends.  Otherwise the next line is a
space-separated list of the elements contained in <i>S<sub>i</sub></i>.

</p><h3>Output</h3>
<p>If [<i>n</i>] cannot be covered by a subcollection of <i>C</i> then
you should output <i>-1</i>, followed by a newline.  Otherwise, your output
should consist of two lines.  The first line is the size
of a minimum-sized set cover.  The second line is a space-separated
list of the 0-based indices of the sets in an optimal set cover.

</p><h3>Example</h3>

<pre><b>Input:</b>
3 4
0
2
2 1
2
1 0
0

<b>Output:</b>
2
1 2
</pre>