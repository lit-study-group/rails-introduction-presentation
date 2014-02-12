##  ArticleのScaffolding

<br>

タイトルと内容を持つArticleを作成する。<br>

<br>

```
rails generate scaffold Article title:string contents:text
```

<br>

＜よく使う型＞

* boolean  (true / false)
* date  (日付)
* datetime  (日付＋時刻)
* float  (小数)
* integer  (整数)
* string  (255文字以内の文字列)
* text  (無制限の文字列)
