<p>Being a completist and a simplist, kid Yang Zhe cannot solve but
  get Wrong Answer from most of the OI problems. And he refuse to
  write two program of same kind at all. So he always failes in
  contests.

</p><p>When having a contest, Yang Zhe looks at the score of every
  problems first. For the problems of the same score, Yang Zhe will
  do only one of them. If he's lucky enough, he can get all the scores
  wanted.

</p><p>Amber is going to hold a contest in SPOJ. She has made a list of
  <i>N</i> candidate problems, which fit Yang Zhe very well. So Yang
  Zhe can solve any problem he want. Amber lined up the problems,
  began to select. She will select a subsequence of the list as the
  final problems. Being A girl of great compassion, she'd like to
  select such a subsequence (can be empty) that Yang Zhe will get the
  maximal score over all the possible subsequences.

</p><p>Amber found the subsequence easily after a few minutes. To make
  things harder, Amber decided that, Yang Zhe can take this contest
  only if Yang Zhe can answer her <i>Q</i> questions. The question is:
  if the final problems are limited to be a subsequence
  of <i>list</i>[<i>X</i>..<i>Y</i>] (1 &lt;= <i>X</i> &lt;= <i>Y</i> &lt;= N),
  what's the maximal possible score Yang Zhe can get?

</p><p>As we know, Yang Zhe is a bit idiot (so why did he solve the
  problem with a negative score?), he got Wrong Answer again... Tell
  him the correct answer!

</p><h3>Input</h3>
<ul>
  <li>Line 1: integer <i>N</i> (1 &lt;= <i>N</i> &lt;= 100000);
  </li><li>Line 2: <i>N</i> integers denoting the score of each problem,
  each of them is a integer in range [-100000, 100000];
  </li><li>Line 3: integer <i>Q</i> (1 &lt;= <i>Q</i> &lt;= 100000);
  </li><li>Line 3+<i>i</i> (1 &lt;= <i>i</i> &lt;= <i>Q</i>): two
  integers <i>X</i> and
  <i>Y</i> denoting the <i>i</i>th question.
</li></ul>

<h3>Output</h3>
<ul>
  <li>Line <i>i</i>: a single integer, the answer to the <i>i</i>th
  question.
</li></ul>

<h3>Example</h3>

<pre><b>Input:</b>
9
4 -2 -2 3 -1 -4 2 2 -6
3
1 2
1 5
4 9

<b>Output:</b>
4
5
3

</pre>
<b>Warning: large input/output data,be careful with certain languages</b>