##  シードデータの作成

<br>

メンバー全員に同じデータを入力させる？<br>
→ シードデータをデータベースにインポートする。

<br>

db/seeds.rb
```
Article.delete_all    # Articleの全消去

Article.create(       # 新規Article作成
  title: 'この勉強会…',
  contents: '楽しく参加してくれてるかな？'
)

```