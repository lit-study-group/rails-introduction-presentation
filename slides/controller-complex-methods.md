## コントローラのメソッド

* 作成するためのメソッドはもう少しだけ複雑.
* どのパラメータを受け取るかを決める
* モデル作れたかによって表示するものを変える

```ruby
class SitesController < ApplicationController
  ...
  def create
    @site = Site.new(site_params)
    if @site.save
      redirect_to @site
    else
      render :new  # redirect_to 'http://yahoo.co.jp'にすると？
    end
  end
  ...
  private
  def site_params
    params.require(:site).permit(:url)
  end
end
```
