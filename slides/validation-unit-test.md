##  ユニットテスト

<br>

モデルのテストを自動化する。<br>

<br>

test/models/article_test.rb
```
  test "title and contents must not be empty" do
    article = Article.new                  # 空のArtcileを生成
    assert article.invalid?                # 何らかのエラーがある確認
    assert article.errors[:title].any?     # titleにエラーがある確認
    assert article.errors[:contents].any?  # contentsにエラーがある確認
  end
```

