<p>
<script type="text/x-mathjax-config">// <![CDATA[
MathJax.Hub.Config({tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}});
// ]]></script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
</p>
    <p>Nested quotations are great not only for writing literature
    with a complex narrative structure, but also in programming
    languages. While it may seem necessary to use different
    quotation marks at different nesting levels for clarity, there
    is an alternative. We can display various nesting levels using
    $k$-quotations, which are
    defined as follows.</p>

    <p>A $1$-quotation is a
    string that begins with a quote character, ends with another
    quote character and contains no quote characters in-between.
    These are just the usual (unnested) quotations. For example,
    <tt class="ttfamily">'this is a string'</tt> is a 
    $1$-quotation.</p>

    <p>For $k &gt; 1$, a
    $k$-quotation is a string
    that begins with $k$ quote
    characters, ends with another 
    $k$ quote characters and contains a
    nested string in-between. The nested string is a non-empty
    sequence of <span style="width:" class="mbox">
    $(k-1)$-quotations, which may
    be preceded, separated, and/or succeeded by any number of
    non-quote characters. For example, <tt class="ttfamily">''All
    'work' and no 'play'''</tt> is a 
    $2$-quotation.</span></p>

    <p>Given a description of a string, you must determine its
    maximum possible nesting level.</p>

    <h3>Input</h3>
    <p>
    Multiple test cases. Please process until EOF is reached. For each test case:</p>
    <p>The input consists of two lines. The first line contains an
    integer $n$ (
    $1 \le n \le 100$). The second line
    contains $n$ integers
    $a_1, a_2, \ldots , a_ n$
    ($1 \le a_ i \le 100$),
    which describe a string as follows. The string starts with
    $a_1$ quote characters,
    which are followed by a positive number of non-quote
    characters, which are followed by 
    $a_2$ quote characters, which are
    followed by a positive number of non-quote characters, and so
    on, until the string ends with 
    $a_ n$ quote characters.</p>

    <h3>Output</h3>

    <p>For each test case, display the largest number 
    $k$ such that a string described by
    the input is a 
    $k$-quotation. If there is no such
    $k$, display <tt class="tt">no quotation</tt> instead.</p>
<h3>Example</h3>
<pre><b>Input:</b>
5
2 1 1 1 3
1
22
1
1

<b>Output:</b>
2
4
no quotation
</pre>