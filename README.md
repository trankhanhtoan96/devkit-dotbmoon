# Mục lục
1. [Các kỹ thuật xử lý giao diện](#1-cc-k-thut-x-l-giao-din)
    1. [Grid system](#i-grid-system)
    2. [Label](#ii-label)
    3. [Icon](#iii-icons)
    4. [Button](#iv-button)

# 1. Các kỹ thuật xử lý giao diện

## i. Grid system

Giao diện được chia làm 12 cột trên 1 hàng ngang.

* general

```html
<div class="row-fluid">
  <div class="span4">...</div>
  <div class="span8">...</div>
</div>
```

* offset

```html
<div class="row-fluid">
  <div class="span4">...</div>
  <div class="span4 offset4">...</div>
</div>
```

* child grid of a column 

```html
<div class="row-fluid">
  <div class="span6">
    Level 1 of column 1
    <div class="row-fluid">
        <div class="span6">Level 2</div>
        <div class="span6">Level 2</div>
    </div>
  </div>
  <div class="span6">
    Level 1 of column 2
  </div>
</div>
```

* Ngoài ra, có thể sử dụng thẻ div với class `.container-fluid` để padding.

```html
<div class="container-fluid">
  <div class="row-fluid">
    <div class="span8">
      <!--Body content-->
    </div>
    <div class="span4">
      <!--Sidebar content-->
    </div>
  </div>
</div>
```

## ii. Label

```html
<span class="label">Default</span>
<span class="label label-important">Important</span>
<span class="label label-warning">warning</span>
<span class="label label-pending">warning</span>
<span class="label label-success">Success</span>
<span class="label label-info">Info</span>
<span class="label label-inverse">Inverse</span>
```

## iii. Icons

các icon ở đây là font-awesome phiên bản 4.2. xem danh sách trong link bên dưới.

https://codepen.io/devmount/details/dPOWgv

## iv. Button

Có các loại button sau: 
- btn
- btn-primary
- btn-info
- btn-success
- btn-warning
- btn-danger
- btn-inverse
- btn-link 

Cách sử dụng: chèn các class trên vào các thẻ a,button,input mà bạn muốn apply css của button đó vào. Lưu ý class `btn` là bắt buộc đi kèm.

```html
<a class="btn" href="">Link</a>
<button class="btn btn-success" type="submit">Button</button>
<input class="btn btn-primary" type="button" value="Input">
<input class="btn btn-danger" type="submit" value="Submit">
```

Button size: `btn-large`, `btn-small`, `btn-mini`

Button fullwidth: `.btn-block`

Button disabled: `.disabled`

Invisible button background: `.btn-invisible`

Button groupd: 

```html
<div class="btn-group">
  <a class="btn">1</a>
  <a class="btn">2</a>
  <a class="btn">3</a>
</div>
```

```html
<div class="btn-toolbar">
  <div class="btn-group">
    ...
  </div>
</div>
```

Button dropdown:

```html
<div class="btn-group">
  <a class="btn dropdown-toggle" data-toggle="dropdown">
    Action
    <i class="fa fa-caret-down"></i>
  </a>
  <ul class="dropdown-menu">
    <!-- dropdown menu links -->
  </ul>
</div>
```

Split button dropdowns:

```html
<div class="btn-group">
  <a class="btn">Action</a>
  <a class="btn dropdown-toggle" data-toggle="dropdown">
    <i class="fa fa-caret-down"></i>
  </a>
  <ul class="dropdown-menu">
    <!-- dropdown menu links -->
  </ul>
</div>
```

