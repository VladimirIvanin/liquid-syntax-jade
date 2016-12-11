# Синтаксис liquid в виде jade/pug миксинов

## for

Пример
```jade
.row
  +for('product', 'collection.products')
  .cell-3
    +include('product-card')
  +endFor()
```
Результат
```liquid
<div class="row">
{% for product in collection.products %}
  <div class="cell-3">
{% include 'product-card'  %}
  </div>
{% endfor %}
</div>
```
