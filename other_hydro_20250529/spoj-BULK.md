<p>ACM uses a&nbsp;new special technology of building its transceiver stations. This technology is called <em>Modular Cuboid Architecture</em> (<em>MCA</em>) and is covered by a&nbsp;patent of Lego company. All parts of the transceiver are shipped in unit blocks that have the form of cubes of exactly the same size. The cubes can be then connected to each other. The MCA is modular architecture, that means we can select preferred transceiver configuration and buy only those components we need .</p>
<p>The cubes must be always connected "face-to-face", i.e. the whole side of one cube is connected to the whole side of another cube. One cube can be thus connected to at most six other units. The resulting equipment, consisting of unit cubes is called <em>The Bulk</em> in the communication technology slang.</p>
<p>Sometimes, an&nbsp;old and unneeded bulk is condemned, put into a&nbsp;storage place, and replaced with a&nbsp;new one. It was recently found that ACM has many of such old bulks that just occupy space and are no longer needed. The director has decided that all such bulks must be disassembled to single pieces to save some space. Unfortunately, there is no documentation for the old bulks and nobody knows the exact number of pieces that form them. You are to write a&nbsp;computer program that takes the bulk description and computes the number of unit cubes.</p>
<p>Each bulk is described by its faces (sides). A&nbsp;special X-ray based machine was constructed that is able to localise all faces of the bulk in the space, even the inner faces, because the bulk can be partially hollow (it can contain empty spaces inside). But any bulk must be connected (i.e. it cannot drop into two pieces) and composed of whole unit cubes.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>There is a&nbsp;single positive integer <var>T</var> on the first line of input (equal to about 1000). It stands for the number of bulks to follow. Each bulk description begins with a&nbsp;line containing single positive integer <var>F</var>, 6 &lt;= <var>F</var> &lt;= 250, stating the number of faces. Then there are <var>F</var> lines, each containing one face description. All faces of the bulk are always listed, in any order. Any face may be divided into several distinct parts and described like if it was more faces. Faces do not overlap. Every face has one inner side and one outer side. No side can be "partially inner and partially outer".</p>
<p>Each face is described on a&nbsp;single line. The line begins with an&nbsp;integer number <var>P</var> stating the number of points that determine the face, 4 &lt;= <var>P</var> &lt;= 200. Then there are 3 <var>x P</var> numbers, coordinates of the points. Each point is described by three coordinates <var>X</var>,<var>Y</var>,<var>Z</var> (0 &lt;= <var>X</var>,<var>Y</var>,<var>Z</var> &lt;= 1000) separated by spaces. The points are separated from each other and from the number <var>P</var> by two space characters. These additional spaces were added to make the input more human readable. The face can be constructed by connecting the points in the specified order, plus connecting the last point with the first one.</p>
<p>The face is always composed of "unit squares", that means every edge runs either in <var>X</var>, <var>Y</var> or <var>Z</var>-axis direction. If we take any two neighbouring points <var>X</var><sub>1</sub>,<var>Y</var><sub>1</sub>,<var>Z</var><sub>1</sub> and   <var>X</var><sub>2</sub>,<var>Y</var><sub>2</sub>,<var>Z</var><sub>2</sub>, then the points will always differ in exactly one of the three coordinates. I.e. it is either  <var>X</var><sub>1</sub> &lt;&gt; <var>X</var><sub>2</sub>, or  <var>Y</var><sub>1</sub> &lt;&gt; <var>Y</var><sub>2</sub>, or   <var>Z</var><sub>1</sub> &lt;&gt; <var>Z</var><sub>2</sub>, other two coordinates are the same. Every face lies in an&nbsp;orthogonal plane, i.e. exactly one coordinate is always the same for all points of the face. The face outline will never touch nor cross itself.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>Your program must print a&nbsp;single line for every test case. The line must contain the sentence <tt>The bulk is composed of </tt><var>V</var><tt> units.</tt>, where <var>V</var> is the volume of the bulk.</p>
<h3>Example</h3>
<p>Sample Input:</p>
<pre><tt>2
12
4  10 10 10  10 10 20  10 20 20  10 20 10
4  20 10 10  20 10 20  20 20 20  20 20 10
4  10 10 10  10 10 20  20 10 20  20 10 10
4  10 20 10  10 20 20  20 20 20  20 20 10
4  10 10 10  10 20 10  20 20 10  20 10 10
5  10 10 20  10 20 20  20 20 20  20 15 20  20 10 20
4  14 14 14  14 14 16  14 16 16  14 16 14
4  16 14 14  16 14 16  16 16 16  16 16 14
4  14 14 14  14 14 16  16 14 16  16 14 14
4  14 16 14  14 16 16  16 16 16  16 16 14
4  14 14 14  14 16 14  16 16 14  16 14 14
4  14 14 16  14 16 16  16 16 16  16 14 16
12
4  20 20 30  20 30 30  30 30 30  30 20 30
4  10 10 10  10 40 10  40 40 10  40 10 10
6  10 10 20  20 10 20  20 30 20  30 30 20  30 40 20  10 40 20
6  20 10 20  20 20 20  30 20 20  30 40 20  40 40 20  40 10 20
4  10 10 10  40 10 10  40 10 20  10 10 20
4  10 40 10  40 40 10  40 40 20  10 40 20
4  20 20 20  30 20 20  30 20 30  20 20 30
4  20 30 20  30 30 20  30 30 30  20 30 30
4  10 10 10  10 40 10  10 40 20  10 10 20
4  40 10 10  40 40 10  40 40 20  40 10 20
4  20 20 20  20 30 20  20 30 30  20 20 30
4  30 20 20  30 30 20  30 30 30  30 20 30
</tt>
</pre>
<p>Sample Output:</p>
<pre><tt>The bulk is composed of 992 units.
The bulk is composed of 10000 units.</tt>
</pre>
<p><strong>Warning: large Input/Output data, be careful with certain languages</strong></p>