##  ビューの変更

<br>

* カテゴリを選択できるようにする<br>

app/views/articles/_form.html.erb
```
  <div class="field">
    <%= f.label :category_id %>
    <%= f.select :category_id, @categories.map{|t| [t.title, t.id]} %>
  </div>
```

<br>

* 一覧に表示する<br>

app/views/articles/index.html.erb
```
…
  <th>Category</th>
…
  <td><%= article.category.title if article.category %></td>
…
```