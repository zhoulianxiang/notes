## redirect and tee
<pre><code>lian@sw:~$ ls > tmp 2>&1
lian@sw:~$ ls 2>&1 | tee tmp
</code></pre>
