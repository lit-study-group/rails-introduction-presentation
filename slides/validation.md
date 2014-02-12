##  バリデーション

<br>

タイトル入力した？コンテンツもある？<br>
タイトル、他のタイトルと被ってない？

<br>

app/models/article.rb

```
class Article < ActiveRecord::Base
  validates :title, :contents, presence: true  # 必ず存在する
  validates :title, uniqueness: true           # 一意である
end
```
