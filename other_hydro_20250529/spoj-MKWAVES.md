<p>Suppose we know a signal is generated by the function x sin (<i>f<sub>1</sub>t</i>) sin (<i>f<sub>2</sub>t</i>). F1 and f2 are two unique
frequencies, each having an integral value in the range 400 to 600 Hz (Hz = cycles per second), and t
represents time. In this problem, you will be given N samples of this function at equally-spaced time
intervals corresponding to t = 1/N, t = 2/N, and so forth. From these samples, you are to determine f1 and
f2.

</p><p></p><p>
For example, suppose f1 = 400 Hz, f2 = 500 Hz, and N = 100. The first sample, at time t = 1/100 sec, is
equal to sin(400 0.01) sin(500 0.01) sin(4) sin(5) 0.156912 . Similarly, the second sample, at
time t = 2/100 sec, is equal to sin(400 0.02) sin(500 0.02) sin(8) sin(10) 0.312821.

</p><h3>Input</h3>
<p>There will be multiple cases to consider. Each case begins with an integer N, no larger than 1000, that
specifies the number of signal samples. The next N data items are real numbers representing the signal
samples at time 1/N sec, 2/N sec, and so forth. A single integer 0 follows the last case.</p><p></p><p>
The number of samples for each case is guaranteed to be sufficient to allow the correct result to be
obtained.

</p><h3>Output</h3>
<p>For each input case, display a single line that is formatted like this:</p><p>
Case 1, f1 = 400, f2 = 500

</p><h3>Example</h3>

<pre><b>Input:</b>
100
0.156912 0.312821 0.466731 0.617657 0.764638 0.906737 1.04305 1.17271
1.29489 1.40883 1.51381 1.60917 1.69432 1.76873 1.83195 1.8836 1.92338
1.95106 1.96649 1.96962 1.96045 1.93908 1.9057 1.86055 1.80396 1.73634
1.65816 1.56997 1.47237 1.36603 1.25166 1.13003 1.00196 0.868307 0.729943
0.587785 0.442764 0.295823 0.147918 1.68756e-010 -0.146981 -0.292088
-0.434403 -0.573031 -0.707107 -0.835801 -0.958325 -1.07394 -1.18195
-1.28171 -1.37266 -1.45428 -1.52611 -1.58779 -1.63898 -1.67947 -1.70907
-1.7277 -1.73535 -1.73205 -1.71795 -1.69323 -1.65816 -1.61308 -1.55838
-1.49452 -1.42201 -1.34141 -1.25334 -1.15846 -1.05745 -0.951057 -0.840028
-0.725146 -0.607206 -0.487017 -0.365392 -0.243145 -0.121082 -2.75143e-010
0.119322 0.236125 0.34968 0.459289 0.564288 0.664055 0.758014 0.845635
0.926438 1 1.06595 1.12398 1.17384 1.21533 1.24833 1.27276 1.28862
1.29596 1.29489 1.28558

0

<b>Output:</b>
Case 1, f1 = 400, f2 = 500
</pre>