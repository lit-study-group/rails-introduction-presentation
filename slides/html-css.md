## HTMLとCSSの基礎

* **HTML**はウェブページの**中身**
* **CSS**はウェブページの**見た目**

<br style="clear: both;">

<div class="half left">
<h3>HTML</h3>
<pre><code>
&lt;html&gt;
  &lt;head&gt;
    &lt;title&gt;私のサイト&lt;/title&gt;
  &lt;head&gt;
  &lt;body&gt;
    &lt;h1 class=&quot;purple&quot;&gt;
      私のサイトへようこそ
    &lt;/h1&gt;
    &lt;div id=&quot;main&quot;&gt;
      &lt;p class=&quot;centered&quot;&gt;
        HTML勉強中です。
      &lt;/p&gt;
    &lt;/div&gt;
  &lt;/body&gt;
&lt;/html&gt;
</code></pre>
</div>

<div class="half right">
<h3>CSS</h3>
<pre><code>
#main {
  margin: 0 auto;
  width: 80%;
}

.purple {
  color: #aa00aa;
}

.centered {
  margin: auto;
  display: block;
}
</code></pre>
</div>
