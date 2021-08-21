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
    * text-muted (灰色)
    * text-primary (藍色)
    * text-success (綠色)
    * text-info (藍綠色)
    * text-warning (黃色)
    * text-danger (紅色)
    * text-secondary (灰色)
    * text-white (白色)
    * text-dark (深灰色)
    * text-body (通常為黑色)
    * text-light (亮灰色)

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
就這樣寫！相信大家國小數學都沒有忘記吧。

好！今天就先這樣，我要去玩overcooked2了🤪