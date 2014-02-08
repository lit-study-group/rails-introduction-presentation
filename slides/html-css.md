## HTMLとCSSの基礎

* **HTML**はウェブページの**中身**
* **CSS**はウェブページの**見た目**

<br class="clear">

<div class="half left">
<h4>HTML</h4>
<pre><code data-trim>
&lt;html&gt;
  &lt;head&gt;
    &lt;title&gt;私のサイト&lt;/title&gt;
    &lt;meta charset=&quot;utf-8&quot;&gt;
    &lt;link rel=&quot;stylesheet&quot; href=&quot;./style.css&quot;&gt;
  &lt;head&gt;
  &lt;body&gt;
    &lt;div id=&quot;main&quot;&gt;
      &lt;h1 class=&quot;purple&quot;&gt;
        私のサイトへようこそ
      &lt;/h1&gt;
      &lt;p class=&quot;large&quot;&gt;
        HTML勉強中です。
      &lt;/p&gt;
    &lt;/div&gt;
  &lt;/body&gt;
&lt;/html&gt;
</code></pre>
</div>

<div class="half right">
<h4>CSS</h4>
<pre><code data-trim>
/\* style.css \*/
#main {
  margin: 0 auto;
  width: 80%;
}

.purple {
  color: #aa00aa;
}

.large {
  font-size: 15pt;
}
</code></pre>
</div>
