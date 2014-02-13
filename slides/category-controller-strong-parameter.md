##  ストロングパラメーター

<br>

不正な値を投げられないような仕組み<br>

<br>

app/controllers/articles_controller.rb
```
    def article_params
      params.require(:article).permit(:title, :contents, :category_id)
    end
```