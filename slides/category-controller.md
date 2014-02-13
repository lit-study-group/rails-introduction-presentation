##  コントローラの変更

<br>

カテゴリ一覧を取得して、ビューに渡す<br>

<br>

app/controllers/articles_controller/_form.html.erb
```
  def new
    @article = Article.new
    @categories = Category.all
  end

  def edit
    @categories = Category.all
  end
```