<h2 id="code-block">Code Block</h2>
<p>This code is from earlier this year and it calculate the volume of a cylinder.
import math</p>
<p>areaperpint = 400/8</p>
<p>while(True):
    radius = float(input(&quot;Enter radius of cylinder : &quot;))
    height = float(input(&quot;Enter height of cylinder : &quot;))
    costperpint = float(input(&quot;Enter cost per pint : &quot;))</p>
<pre><code><span class="hljs-keyword">if</span> (radius &lt; <span class="hljs-number">0</span> <span class="hljs-keyword">or</span> height &lt; <span class="hljs-number">0</span> <span class="hljs-keyword">or</span> costperpint &lt; <span class="hljs-number">0</span>):
    <span class="hljs-keyword">print</span>(<span class="hljs-string">"Invalid Input"</span>)
    <span class="hljs-keyword">continue</span>

area = (<span class="hljs-number">2</span> * math.<span class="hljs-built_in">pi</span> * radius) * (height + radius)
totalpints = math.<span class="hljs-built_in">ceil</span>(area/areaperpint)
totalcost =totalpints * costperpint

<span class="hljs-keyword">print</span>(<span class="hljs-string">"Total Cost :$"</span>, <span class="hljs-built_in">round</span>(totalcost,<span class="hljs-number">2</span>))
<span class="hljs-keyword">print</span>(<span class="hljs-string">"Total Pints :"</span>, totalpints)

morecalc = input(<span class="hljs-string">"Do you want another calculation (Y/N): "</span>)

<span class="hljs-keyword">if</span> morecalc.<span class="hljs-built_in">upper</span>() == 'Y':
    <span class="hljs-keyword">continue</span>
<span class="hljs-keyword">else</span>:
    <span class="hljs-keyword">break</span>
</code></pre><p>*<a href="./README.md">Home Page</a></p>
