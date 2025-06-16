<p><span style="color: #333333; font-family: 'Helvetica Neue', Helvetica, 'Segoe UI', Arial, freesans, sans-serif; font-size: 16px; line-height: 25.6px;">Let&nbsp;</span><strong>F(n)</strong><span style="color: #333333; font-family: 'Helvetica Neue', Helvetica, 'Segoe UI', Arial, freesans, sans-serif; font-size: 16px; line-height: 25.6px;">&nbsp;be the&nbsp;</span><strong><em>n<sup>th</sup>&nbsp;member of the&nbsp;</em>Fibonacci sequence</strong><span style="color: #333333; font-family: 'Helvetica Neue', Helvetica, 'Segoe UI', Arial, freesans, sans-serif; font-size: 16px; line-height: 25.6px;">:</span></p>
<pre style="box-sizing: border-box; overflow: auto; font-family: Consolas, 'Liberation Mono', Menlo, Courier, monospace; font-size: 13.6px; margin-top: 0px; margin-bottom: 16px; font-stretch: normal; line-height: 1.45; padding: 16px; border-radius: 3px; word-wrap: normal; color: #333333; background-color: #f7f7f7;"><code style="box-sizing: border-box; font-family: Consolas, 'Liberation Mono', Menlo, Courier, monospace; font-size: 13.6px; padding: 0px; margin: 0px; border-radius: 3px; word-break: normal; border: 0px; display: inline; max-width: initial; overflow: initial; line-height: inherit; word-wrap: normal; background: transparent;">F(<span style="box-sizing: border-box;">0) = <span style="box-sizing: border-box; color: #008080;">0</span>, <span style="box-sizing: border-box; font-weight: bold;">F</span>(<span style="box-sizing: border-box; color: #008080;">1</span>) = <span style="box-sizing: border-box; color: #008080;">1</span>,  
<span style="box-sizing: border-box; font-weight: bold;">F</span>(<span style="box-sizing: border-box; font-weight: bold;">n</span>) = <span style="box-sizing: border-box; font-weight: bold;">F</span>(<span style="box-sizing: border-box; font-weight: bold;">n</span>-<span style="box-sizing: border-box; color: #008080;">1</span>)+<span style="box-sizing: border-box; font-weight: bold;">F</span>(<span style="box-sizing: border-box; font-weight: bold;">n</span>-<span style="box-sizing: border-box; color: #008080;">2</span>) (<span style="box-sizing: border-box; font-weight: bold;">n</span> &gt; <span style="box-sizing: border-box; color: #008080;">1</span>)</span></code></pre>
<p style="box-sizing: border-box; margin-top: 0px; margin-bottom: 16px; color: #333333; font-family: 'Helvetica Neue', Helvetica, 'Segoe UI', Arial, freesans, sans-serif; font-size: 16px; line-height: 25.6px;">Consider the following Fibonacci polynomial:</p>
<p style="box-sizing: border-box; margin-top: 0px; margin-bottom: 16px; color: #333333; font-family: 'Helvetica Neue', Helvetica, 'Segoe UI', Arial, freesans, sans-serif; font-size: 16px; line-height: 25.6px;">A(x) = x F(1) + x<sup>2</sup>&nbsp;F(2) + x<sup>3</sup>&nbsp;F(3) + ... + x<sup>n</sup>&nbsp;F(n) + ....<br style="box-sizing: border-box;">= sigma(n = 0 to infinity) x<sup>n</sup>&nbsp;F(n)</p>
<p style="box-sizing: border-box; margin-top: 0px; margin-bottom: 16px; color: #333333; font-family: 'Helvetica Neue', Helvetica, 'Segoe UI', Arial, freesans, sans-serif; font-size: 16px; line-height: 25.6px;">Amazingly,</p>
<p style="box-sizing: border-box; margin-top: 0px; margin-bottom: 16px; color: #333333; font-family: 'Helvetica Neue', Helvetica, 'Segoe UI', Arial, freesans, sans-serif; font-size: 16px; line-height: 25.6px;">A(1/2) = 1/2 + 1/2<sup>2</sup>&nbsp;+ 2/2<sup>3</sup>&nbsp;+ 3/2<sup>4</sup>&nbsp;+ .... + F(n)/2<sup>n</sup>&nbsp;+ ... = 2</p>
<p style="box-sizing: border-box; margin-top: 0px; margin-bottom: 16px; color: #333333; font-family: 'Helvetica Neue', Helvetica, 'Segoe UI', Arial, freesans, sans-serif; font-size: 16px; line-height: 25.6px;"><span style="line-height: 25.6px;">In this problem, we only considering the non-negative-integer value of&nbsp;</span><code style="box-sizing: border-box; font-family: Consolas, 'Liberation Mono', Menlo, Courier, monospace; font-size: 13.6px; padding: 0.2em 0px; margin: 0px; border-radius: 3px; background-color: rgba(0, 0, 0, 0.0392157);">A(x)</code><span style="line-height: 25.6px;">. Here are some examples of&nbsp;</span><code style="box-sizing: border-box; font-family: Consolas, 'Liberation Mono', Menlo, Courier, monospace; font-size: 13.6px; padding: 0.2em 0px; margin: 0px; border-radius: 3px; background-color: rgba(0, 0, 0, 0.0392157);">A(x)</code><span style="line-height: 25.6px;">&nbsp;for specific&nbsp;</span><code style="box-sizing: border-box; font-family: Consolas, 'Liberation Mono', Menlo, Courier, monospace; font-size: 13.6px; padding: 0.2em 0px; margin: 0px; border-radius: 3px; background-color: rgba(0, 0, 0, 0.0392157);">x</code><span style="line-height: 25.6px;">.</span></p>
<table style="box-sizing: border-box; border-collapse: collapse; border-spacing: 0px; margin-top: 0px; margin-bottom: 16px; display: block; width: 293px; overflow: auto; word-break: keep-all; color: #333333; font-family: 'Helvetica Neue', Helvetica, 'Segoe UI', Arial, freesans, sans-serif; font-size: 16px; line-height: 25.6px;" border="0">
<tbody style="box-sizing: border-box;">
<tr style="box-sizing: border-box; border-top-width: 1px; border-top-style: solid; border-top-color: #cccccc;">
<th style="box-sizing: border-box; padding: 6px 13px; border: 1px solid #dddddd;">x</th><th style="box-sizing: border-box; padding: 6px 13px; border: 1px solid #dddddd;">A(x)</th>
</tr>
<tr style="box-sizing: border-box; border-top-width: 1px; border-top-style: solid; border-top-color: #cccccc; background-color: #f8f8f8;">
<td style="box-sizing: border-box; padding: 6px 13px; border: 1px solid #dddddd;">0</td>
<td style="box-sizing: border-box; padding: 6px 13px; border: 1px solid #dddddd;">0</td>
</tr>
<tr style="box-sizing: border-box; border-top-width: 1px; border-top-style: solid; border-top-color: #cccccc;">
<td style="box-sizing: border-box; padding: 6px 13px; border: 1px solid #dddddd;">sqrt(2)-1</td>
<td style="box-sizing: border-box; padding: 6px 13px; border: 1px solid #dddddd;">1</td>
</tr>
<tr style="box-sizing: border-box; border-top-width: 1px; border-top-style: solid; border-top-color: #cccccc; background-color: #f8f8f8;">
<td style="box-sizing: border-box; padding: 6px 13px; border: 1px solid #dddddd;">1/2</td>
<td style="box-sizing: border-box; padding: 6px 13px; border: 1px solid #dddddd;">2</td>
</tr>
<tr style="box-sizing: border-box; border-top-width: 1px; border-top-style: solid; border-top-color: #cccccc;">
<td style="box-sizing: border-box; padding: 6px 13px; border: 1px solid #dddddd;">[sqrt(13)-2]/3</td>
<td style="box-sizing: border-box; padding: 6px 13px; border: 1px solid #dddddd;">3</td>
</tr>
<tr style="box-sizing: border-box; border-top-width: 1px; border-top-style: solid; border-top-color: #cccccc; background-color: #f8f8f8;">
<td style="box-sizing: border-box; padding: 6px 13px; border: 1px solid #dddddd;">[sqrt(89)-5]/8</td>
<td style="box-sizing: border-box; padding: 6px 13px; border: 1px solid #dddddd;">4</td>
</tr>
</tbody>
</table>
<p><span style="color: #333333; font-family: 'Helvetica Neue', Helvetica, 'Segoe UI', Arial, freesans, sans-serif; font-size: 16px; line-height: 25.6px;">Find out if&nbsp;</span><code style="box-sizing: border-box; font-family: Consolas, 'Liberation Mono', Menlo, Courier, monospace; font-size: 13.6px; padding: 0.2em 0px; margin: 0px; border-radius: 3px; background-color: rgba(0, 0, 0, 0.0392157);">x</code><span style="color: #333333; font-family: 'Helvetica Neue', Helvetica, 'Segoe UI', Arial, freesans, sans-serif; font-size: 16px; line-height: 25.6px;">&nbsp;is rational with the given value of&nbsp;</span><code style="box-sizing: border-box; font-family: Consolas, 'Liberation Mono', Menlo, Courier, monospace; font-size: 13.6px; padding: 0.2em 0px; margin: 0px; border-radius: 3px; background-color: rgba(0, 0, 0, 0.0392157);">A(x)</code></p>
<h3>Input</h3>
<p><span style="font-size: small;">The first line contains T, the number of test cases. The next T lines contains the value of A(x). </span></p>
<ul style="box-sizing: border-box; padding: 0px 0px 0px 2em; margin-top: 0px; margin-bottom: 0px; color: #333333; font-family: 'Helvetica Neue', Helvetica, 'Segoe UI', Arial, freesans, sans-serif; font-size: 16px; line-height: 25.6px;">
<li style="box-sizing: border-box;"><code style="box-sizing: border-box; font-family: Consolas, 'Liberation Mono', Menlo, Courier, monospace; font-size: 13.6px; padding: 0.2em 0px; margin: 0px; border-radius: 3px; background-color: rgba(0, 0, 0, 0.0392157);">0 &lt;= Ax &lt;= 10^17</code></li>
<li style="box-sizing: border-box;"><code style="box-sizing: border-box; font-family: Consolas, 'Liberation Mono', Menlo, Courier, monospace; font-size: 13.6px; padding: 0.2em 0px; margin: 0px; border-radius: 3px; background-color: rgba(0, 0, 0, 0.0392157);">1 &lt;= T &lt;= 100000</code></li>
</ul>
<h3>Output</h3>
<ul style="box-sizing: border-box; padding: 0px 0px 0px 2em; margin-top: 0px; margin-bottom: 0px; color: #333333; font-family: 'Helvetica Neue', Helvetica, 'Segoe UI', Arial, freesans, sans-serif; font-size: 16px; line-height: 25.6px;">
<li style="box-sizing: border-box;"><code style="box-sizing: border-box; font-family: Consolas, 'Liberation Mono', Menlo, Courier, monospace; font-size: 13.6px; padding: 0.2em 0px; margin: 0px; border-radius: 3px; background-color: rgba(0, 0, 0, 0.0392157);">1 if the given Ax yeilds a rational x, 0 otherwise</code></li>
</ul>
<h3>Example</h3>
<pre><strong>Input:</strong>
<span style="font-size: small;">5</span></pre>
<pre><span style="font-size: small;">0</span></pre>
<pre><span style="font-size: small;">1</span></pre>
<pre><span style="font-size: small;">2</span></pre>
<pre><span style="font-size: small;">3</span></pre>
<pre><span style="font-size: small;">4</span></pre>
<pre><strong>Output:</strong>
<span style="font-size: small;">1</span></pre>
<pre><span style="font-size: small;">0</span></pre>
<pre><span style="font-size: small;">1</span></pre>
<pre><span style="font-size: small;">0</span></pre>
<pre><span style="font-size: small;">0</span></pre>