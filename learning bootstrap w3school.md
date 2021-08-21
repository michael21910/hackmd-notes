# w3c - Notes Learning Bootstrap

[Reference from w3schools](https://www.w3schools.com/bootstrap4/default.asp)

筆記是我從w3schools邊學邊做筆記的。  
廢話不多說，讓我們開始吧！
  
## BS4 Containers
* Container, Container-fulid
    * 不同的地方在於fulid會水平滿版
* m(margin), p(padding）
    * t, b, l, r 分別代表上、下、左、右，不打表示全都要！
    * x代表左右、y代表上下
    * 程度為1~5
    * Example: mt-4, pr-2, m-1, p-3等等，都可以任意組合！
* 顏色
    * text-muted （灰色）
    * text-primary （藍色）
    * text-success （綠色）
    * text-info （藍綠色）
    * text-warning （黃色）
    * text-danger （紅色）
    * text-secondary （灰色）
    * text-white （白色）
    * text-dark （深灰色）
    * text-body （通常為黑色）
    * text-light （亮灰色）
* 以上的text改成bg，就會變背景顏色！也適用於table！還有btn！

## BS4 Grid Basic
我自己看下來有一點display: flex的感覺啦，還好有先學一點css😅
* 大小區分
    * col-sm(small), col-md(medium), col-lg(large), col-xl

不過要讓他們乖乖排好的話···
```html
<div class="row">
  <div class="col">.col</div>
  <div class="col">.col</div>
  <div class="col">.col</div>
</div>
```
這樣就可以了，簡單明瞭吧！

另外，bootstrap把網頁分成12份。  
所以你想要左邊三分之一，右邊三分之二的話···
```html
<div class="row">
  <div class="col-sm-4">.col-sm-4</div>
  <div class="col-sm-8">.col-sm-8</div>
</div>
```
就這樣寫！  
相信大家國小數學都沒有忘記吧。

## BS4 Typography
就是字體的各種樣式！  
字體大小有一點無聊，我提一些有趣的好了。
* mark
    * <mark>螢光筆！</mark>
* abbr
    * <abbr>炫泡底線，哦不md沒有</abbr>
* dl, dd, dt
    * 很像條列的感覺
    ```html
        <dl>
            <dt>Coffee</dt>
            <dd>- black hot drink</dd>
            <dt>Milk</dt>
            <dd>- white cold drink</dd>
        </dl>  
    ```
* code
    * 會讓文字長得很像<code>code</code>？
    * 那個上面的"code"缺了紅色的顏色哦！
* kbd
    * <kbd>黑底白字</kbd>，oops，md沒有

## BS4 Tables
一樣提一些有趣的！
* table-hover
    * 滑鼠一上去會變灰色，酷

就···就這樣，其他都還好。

## BS4 Jumbotron
這太適合頁面的header了吧吧吧吧吧！
```html
    <div class="jumbotron">
        <h1>Bootstrap Tutorial</h1>
        <p>Bootstrap is the most popular HTML, CSS...</p>
    </div>
```
大大框框，好爽好爽。  
加 <mark>**jumbotron-fulid**</mark> 會變成水平滿版，終了！

## BS4 Buttons
按鈕來啦！！直接上實際語法！
```html
    <button type="button" class="btn btn-(上面提到的顏色)">The Btn</button>
```
* btn-(color)
    * 按鈕變顏色
* btn-outline-(color)
    * 按鈕外面的顏色
* btn-lg, btn-sm
    * 按鈕大小，但感覺用不到
* btn-block
    * 水平滿版btn
* disabled
    * 不能點的按鈕
* spinner-border
    * 按鈕可以加這個，超惱人的loading，好好笑

## BS4 Button groups
完完全全就是navigation bar啊啊啊啊啊！
```html
<div class="btn-group（橫的） / .btn-group-vertical（直的）">
  <button type="button" class="btn btn-primary">Apple</button>
  <button type="button" class="btn btn-primary">Samsung</button>
  <button type="button" class="btn btn-primary">Sony</button>
</div>
```

還有下拉式選單！（我當初設計這個設計的好痛苦啊）  
為甚麼不提早學這個呢😅
```html
<div class="btn-group">
    <button type="button" class="btn btn-primary">Sony</button>
    <button type="button" class="btn btn-primary dropdown-toggle dropdown-toggle-split" data-toggle="dropdown">
      <span class="caret"></span>
    </button>
    <div class="dropdown-menu">
      <a class="dropdown-item" href="#">Tablet</a>
      <a class="dropdown-item" href="#">Smartphone</a>
    </div>
  </div>
```

## BS4 Progress Bars
好香啊···
```html
<div class="progress">
  <div class="progress-bar bg-(color)" style="width:70%">70%</div>
</div>
```
很漂漂！還可以換顏色！

## BS4 Pagination
To Be Continued...