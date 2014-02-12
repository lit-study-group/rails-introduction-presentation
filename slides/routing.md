## ルーティング

* アドレスによってページを決める
* Railsでは使うコントローラを決める
* Railsでは`config/routes.rb`で設定する

```ruby
UrlShortener::Application.routes.draw do
  root to: 'sites#new'
  resources :sites, only: [:show, :create]
  get '/:token', to: 'sites#redirect', as: :redirect
end
```

* `foo#bar`は`FooController`の`bar`メソッドを使う意味表してる.
* `root`はパスがない時. (例: twitter.com/対twitter.com/i/connect)
* `resources :sites`は`SitesController`へのルートの生成
* `get`は`GET`メソッド
* `:token`は`token`という名前で入る任意パラメータ
* `bundle exec rake routes`ですべてのルートを確認
