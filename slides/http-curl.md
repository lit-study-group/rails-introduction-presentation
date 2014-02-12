## HTTPを試してみる

HTTPサーバーに問い合わせする.

```
curl -v www.google.co.jp
```

<br>

<div class="half left">
<h4>リクエストのヘッダー</h4>
<pre><code data-trim>
GET / HTTP/1.1
User-Agent: curl/7.35.0
Host: www.google.co.jp
Accept: \*/\*
</code></pre>
</div>

<div class="half right">
<h4>レスポンスのヘッダー</h4>
<pre><code data-trim>
HTTP/1.1 200 OK
Date: Wed, 12 Feb 2014 19:27:13 GMT
Expires: -1
Cache-Control: private, max-age=0
Content-Type: text/html; charset=Shift_JIS
Set-Cookie: PREF=ID=9e74633099834b51:FF=0:TM=1392233233:LM=1392233233:S=mh8_gdnNIIdgxgzu; expires=Fri, 12-Feb-2016 19:27:13 GMT; path=/; domain=.google.co.jp
Set-Cookie: NID=67=BUdY0WjZ0k0LBnmxE7nTITXebJTY5Oa0EVfC2bC5FFnzzeqaIGPvIzLzlG522VmGpdtgwJXMoVip-gyeORI_tVaEAsZcd0ZWdfUoTIjzYtS1Pfv0MkyTzCscYxLUJGEt; expires=Thu, 14-Aug-2014 19:27:13 GMT; path=/; domain=.google.co.jp; HttpOnly
P3P: CP="This is not a P3P policy! See http://www.google.com/support/accounts/bin/answer.py?hl=en&answer=151657 for more info."
Server gws is not blacklisted
Server: gws
X-XSS-Protection: 1; mode=block
X-Frame-Options: SAMEORIGIN
Alternate-Protocol: 80:quic
Transfer-Encoding: chunked
</code></pre>
続いてレスポンスの中身
</div>
