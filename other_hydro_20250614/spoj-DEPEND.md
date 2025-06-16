<p>We bought a brand new computer and now we would like to install an operating system. The only problem is that our chosen operating system consists of many packages and they cannot be installed in an arbitrary order. E.g. you cannot install the package tuxracer, which depends on the package libSDL, before you install libSDL. But libSDL can depend on another packages and so on. The packages may only be installed one at a time. You may install a package only if you already installed all packages it depends on. Your task is to determine how many packages can be installed on our computer. </p>

<h3>Input file specification</h3>
<p>The input file contains a single line for each available package. The line for each package P begins with the name of the package. The name of each package is a non-empty string of printable characters containing no spaces. Following the name of the package P is the dependency list of P. The dependency list is simply a list of names of packages that P depends on, separated by spaces. A whitespace followed by a single 0 (zero) is at the end of each line. You may assume that no package has the name '0'. </p>

<p>The dependency list of a package P may be empty; in that case, P does not depend on any packages and may be installed immediately. It is possible that a package Q occurs in the dependency list of a package P more than once; this merely means that P depends on Q, nothing more. Only the packages that have a dependency list in the input file are available and may be installed. It is possible that a package P depends on a package that is not available. Such a package cannot be installed. </p>
<p>The number of lines in the input file will be less than 9000.</p>
<h3>Output file specification</h3>
<p>The output consists of one number -- the maximum number of packages that may be installed on the computer. </p>

<h3>Example</h3>
<pre><b>Input file</b>
a b c b 0
b c 0
c 0
d e f 0
e f 0
f e 0
g h 0

<b>Output file</b>
3
</pre>
<b>Note</b>
<p>Package c can be installed immediately. Package b depends only on c, and hence can also be installed once we installed c. Finally, package a depends only on b and c and can now also be installed. It is easy to verify that no other packages can be installed.</p>