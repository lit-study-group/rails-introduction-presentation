## ビュー

* 基本的に普通のHTMLとCSS
* コントローラから生成される
* 普通のHTMLと違って, 変数の値を入れる必要がある
    * テンプレートエンジンを使う
    * RailsのデフォルトはERB (Embed Ruby)

```
<h1><%= t 'site.shorten_url' %></h1>

<%= form_for @site do |f| %>
  <div class="row">
    <div class="col-lg-1">
      <%= f.label :url, t('site.url') %>
    </div>
    <div class="col-lg-2">
      <%= f.text_field :url %>
    </div>
    <% unless @site.errors[:url].empty? %>
      <div class="col-lg-3 col-lg-offset-1 alert-danger">
        <%= t @site.errors[:url].first %>
      </div>
    <% end %>
  </div>
  <div class="row">
    <div class="col-lg-1">
      <%= f.submit t('btn.shorten'), class: 'btn btn-primary' %>
    </div>
  </div>
<% end %>
```
