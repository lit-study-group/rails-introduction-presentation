## コントローラのメソッド

* `SitesController`から`Site`モデルを使う.
* レスポンスを指定しないと, メソッドと同じ名前のテンプレートが表示される
    * `sites#show`の場合, `views/sites/show.html.erb`
    * `sites#new`の場合, `views/sites/new.html.erb`
    
```ruby
# app/controllers/sites_controller.rb
class SitesController < ApplicationController
  def show
    @site = Site.find(params[:id]) # params[:id]を1に変えると?
  end

  def new
    @site = Site.new(params[:site])
  end
  ...
end
```
