<p>Most nonfiction and reference books have an <em>index</em> to help
readers find references to specific terms or concepts in the text.  Here
is a sample index.</p>

<blockquote><pre>larch, 4, 237, 238, 414
+ Monty Python and, 64, 65, 66
+ planting of, 17
Lenny Kravitz, 50
+ going his way, 53
lumbago, 107
mango
+ Chris Kattan, 380
+ storage of, 87, 90
+ use in Nethack, 500, 501
+ Vitamin C content, 192
</pre></blockquote>

<p>Each index entry contains a <b><i>primary entry</i></b> followed by zero or
more <b><i>secondary entries</i></b>, which begin with a '<tt>+</tt>'.  Entries will
normally be followed by a list of page references, but a primary entry
might not be if at least one secondary entry is present (as is the case
with <i>mango</i>, above).  Primary entries are sorted, and secondary
entries following a primary entry are also sorted. Sorting is
case-insensitive.  Page references for an entry are in ascending order
and do not include duplicates. (A duplicate could occur if there are two
or more identical entries on the same page.)</p>

<p>Your task is to read a document that has index information embedded
within it and produce the index.  Documents consist of one or more
lines of ASCII text. The page number starts at 1, and the character
'<tt>&amp;</tt>' indicates the start of a new page (which adds 1 to the current
page number).  Index entries are indicated by a <b><i>marker</i></b>, which in
its most elaborate form has the following syntax:</p>

<blockquote>{<i>text</i><tt>%</tt><i>primary</i><tt>$</tt><i>secondary</i>}
</blockquote>

<p>Here <i>text</i> is the text to be indexed, <i>primary</i> is an
alternative primary entry, and <i>secondary</i> is a secondary entry.
Both '<tt>%</tt><i>primary</i>' and '<tt>$</tt><i>secondary</i>' are optional,
but if
both are present they must appear in the order given.  If <i>primary</i>

is present then it is used as the primary entry, and if not then <i>text</i> is used as the primary entry.  If <i>secondary</i> is present then
the marker adds a page reference for that secondary entry; otherwise it
adds a page reference for the primary entry.  A single marker cannot
add a page reference for both a primary and secondary entry. Here are
examples of each of the four possible types of marker, which correspond
to four of the entries in the sample index above.</p>

<blockquote><pre>... his {lumbago} was acting up, so ...
... {Lenny%Lenny Kravitz} lit up the crowd with his version of ...
... Monty Python often used the {larch$Monty Python and} in ...
... when storing {mangos%mango$storage of}, be sure to ...
</pre></blockquote>

<p>The input consists of one or more documents, followed by a line
containing only '<tt>**</tt>' that signals the end of the input.  Documents are
implictly numbered starting with 1. Each document consists of one or
more lines of text followed by a line containing only '<tt>*</tt>'.  Each line
of text will be at most 79 characters long, not counting end-of-line
characters.  For document <i>i</i>, output the line '<tt>DOCUMENT</tt> <i>i</i>' followed
by the sorted index using the exact output format shown in the
examples.</p>

<p>Be sure to read <a href="../notes/teams.html"><i>Notes to Teams</i></a>,
which has general formatting
guidelines that pertain to all problem input files, including this one.
Also note:</p>

<ul>
<li>A document will contain at most 100 markers,
with at most 20 primary entries.</li>
<li>A primary entry will have at most 5 secondary entries.</li>
<li>An entry will have at most 10 unique page references (not including 
        duplicates).</li>
<li>The character '<tt>&amp;</tt>' will not appear anywhere within a marker, and
will appear at most 500 times within a document.</li>
<li>The character '<tt>*</tt>' is used only to signal the end of a document or
the end of the input.</li>

<li>The characters '<tt>{</tt>', '<tt>}</tt>', '<tt>%</tt>', and '<tt>$</tt>' will only be used to
define markers, and will not appear in any text or entries.</li>
<li>A marker may span one or more lines.  Every end-of-line within a
marker must be converted to a single space.</li>
<li>A space within a marker (including a converted end-of-line) is
normally included in the text/entry, just like any other character.
However, any space that immediately follows '<tt>{</tt>', 
immediately precedes '<tt>}</tt>', or is immediately adjacent to '<tt>%</tt>' or '<tt>$</tt>' 
must be ignored.</li>

<li>The total length of a marker, measured from the opening '<tt>{</tt>' to 
the closing '<tt>}</tt>', and in which all embedded end-of-lines are converted
to spaces, will be at most 79 characters.</li>
</ul>


<pre><b>Input:</b>
Call me Ishmael.
*
One {fish $unary}, two {fish$ binary},&amp;red {fish $ scarlet}, blue {fish$
azure}. &amp; By { Dr. Seuss }.
*
This is a {simple } &amp; &amp; { document} that &amp;{
simply %simple
$adverb
} &amp; {illustrates %vision} &amp;&amp;&amp;&amp;&amp; one {simple-minded% simple} {Judge}'s {vision} 
for what a {document } might { look % vision} like.
*
**

</pre>

<pre><b>Output:</b>
DOCUMENT 1
DOCUMENT 2
Dr. Seuss, 3
fish
+ azure, 2
+ binary, 1
+ scarlet, 2
+ unary, 1
DOCUMENT 3
document, 3, 10
Judge, 10
simple, 1, 10
+ adverb, 4
vision, 5, 10
</pre>