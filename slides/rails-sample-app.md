## サンプルアプリ

URLを圧縮するためのアプリ.

```
https://www.google.com/search?q=mvc+rails&ie=utf-8&oe=utf-8&aq=t&rls=org.mozilla:en-US:official&client=firefox-a&channel=sb
->
http://myapp.com/foo
```

ソースコードは[Github](https://github.com/lit-study-group/rails-url-shortener)に公開.

アプリケーションは[Heroku](http://rails-url-shortener.herokuapp.com/)に公開.

アプリをローカルで動かす.

```
git clone https://github.com/lit-study-group/rails-url-shortener.git
cd rails-url-shortener
bundle install --without production
bundle exec rake db:migrate
bundle exec rails server
```

動いたら[http://localhost:3000](http://localhost:3000)を開く.
