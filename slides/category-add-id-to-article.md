##  マイグレーション

<br>

記事にカテゴリIDを加える。<br>
add_XX_to_YYの形のマイグレーション<br>

<br>

```
rails generate migration add_category_id_to_article category_id:integer
rake db:migrate
```

<br>

