<h1 id="weather-observation-station-11">Weather Observation Station 11</h1>
<p><a href="https://www.hackerrank.com/challenges/weather-observation-station-11/problem">Source</a></p>
<p>Query the list of CITY names from STATION that either do not start with vowels or do not end with vowels. Your result cannot contain duplicates.</p>
<p>The STATION table is described as follows:<br>
<img src="https://s3.amazonaws.com/hr-challenge-images/9336/1449345840-5f0a551030-Station.jpg" alt="Station Table Structure" title="Station Table Structure"></p>
<blockquote>
<p>where LAT_N is the northern latitude and LONG_W is the western longitude.</p>
</blockquote>
<h2 id="answer">Answer</h2>
<p>solved by <a href="https://www.github.com/kingrayhan">@KingRayhan</a></p>
<pre class=" language-sql"><code class="prism  language-sql"><span class="token keyword">SELECT</span> <span class="token keyword">DISTINCT</span> city <span class="token keyword">FROM</span> STATION <span class="token keyword">WHERE</span>
<span class="token punctuation">(</span>city <span class="token operator">not</span> <span class="token operator">like</span> <span class="token string">'a%'</span> <span class="token operator">or</span> city <span class="token operator">not</span> <span class="token operator">like</span> <span class="token string">'%a'</span><span class="token punctuation">)</span> <span class="token operator">or</span>
<span class="token punctuation">(</span>city <span class="token operator">not</span> <span class="token operator">like</span> <span class="token string">'e%'</span> <span class="token operator">or</span> city <span class="token operator">not</span> <span class="token operator">like</span> <span class="token string">'%e'</span><span class="token punctuation">)</span> <span class="token operator">or</span>
<span class="token punctuation">(</span>city <span class="token operator">not</span> <span class="token operator">like</span> <span class="token string">'i%'</span> <span class="token operator">or</span> city <span class="token operator">not</span> <span class="token operator">like</span> <span class="token string">'%i'</span><span class="token punctuation">)</span> <span class="token operator">or</span>
<span class="token punctuation">(</span>city <span class="token operator">not</span> <span class="token operator">like</span> <span class="token string">'o%'</span> <span class="token operator">or</span> city <span class="token operator">not</span> <span class="token operator">like</span> <span class="token string">'%o'</span><span class="token punctuation">)</span> <span class="token operator">or</span>
<span class="token punctuation">(</span>city <span class="token operator">not</span> <span class="token operator">like</span> <span class="token string">'u%'</span> <span class="token operator">or</span> city <span class="token operator">not</span> <span class="token operator">like</span> <span class="token string">'%u'</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
</code></pre>

