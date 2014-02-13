##  関連付け

<br>

Category : Article = 1 : N<br>

<br>

app/models/article.rb

```
class Article < ActiveRecord::Base
  belongs_to :category                         # カテゴリに属する
  validates :title, :contents, presence: true  # 必ず存在する
  validates :title, uniqueness: true           # 一意である
end
```

<br>

app/models/category.rb

```
class Category < ActiveRecord::Base
  has_many :articles  # 複数のarticlesを持つ
end
```