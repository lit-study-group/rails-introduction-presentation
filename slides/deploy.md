## Herokuにアップロード

Gemfileで`gem sqlite3`を以下のようにに変える.

```ruby
group :development, :test do
  gem 'sqlite3'
end

group :production do
  gem 'rails_12factor'
  gem 'pg'
end

```

次に

```
bundle install --without production
git init # 1回目だけ
git add .
git commit -m "Initial commit."
heroku create APP_NAME # 1回目だけ
git push heroku master
heroku run rake db:migrate
heroku open
```
