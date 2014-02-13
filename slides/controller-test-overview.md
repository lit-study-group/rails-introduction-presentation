##  機能テストの修正

<br>

以下の修正を加える<br>

<br>

test/controllers/articles_controller_test.rb
```
  setup do
    @article = articles(:one)
    @update = {
      title: 'あっぷでーと',
      contents: 'こんてんつ'
    }
  end

  test "should create article" do
    assert_difference('Article.count') do
      post :create, article: @update
    end

    assert_redirected_to article_path(assigns(:article))
  end

  test "should update article" do
    patch :update, id: @article, article: @update
    assert_redirected_to article_path(assigns(:article))
  end
```
