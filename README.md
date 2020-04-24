
# HTMLテスト

### Q1
#### 正しい記述を選択してください。
図A
```
.
├── public   
│   └── assets  
│          ├── css 
│          │    └── common.css
│          │    └── auth.css
│          │    └── mypage.css
│          └── img
│               ├── auth
│               │     └── top.png
│               │     └── icon.png
│               │     └── banner.png
│               └── mypage
│                     └── top.png
│                     └── icon.png
│                     └── dammy1.png
└── src 
    ├── auth.php
    └── mypage.php
    └── menu.php
```
図Aのディレクトリのmypage.phpに同じディレクトリにある画像とCSSを適用させます。  
正しいパスである組み合わせを選んでください。
- 画像　./public/assets/img/mypage/top.png
- CSS　./public/assets/css/common.css

```html
1. <img src="../../public/assets/img/mypage/icon.png">  
   <link rel="stylesheet" type="text/css" href="/public/assets/css/mypage.css">

2. <img src="../../public/assets/img/mypage/icon.png">  
   <link rel="stylesheet" type="text/css" href="../public/assets/css/mypage.css">

3. <img src="../public/assets/img/mypage/icon.png">  
   <link rel="stylesheet" type="text/css" href="/public/assets/css/mypage.css">

4. <img src="/public/assets/img/mypage/icon.png">  
   <link rel="stylesheet" type="text/css" href="../public/assets/css/mypage.css">

5. 全て当てはまる

6. 該当なし
```
### Q2
#### 誤っている記述を選択してください。
```html
1. <a href="">のhref属性はクリックした際のリンク先を指定する
2. <a href="">のhref属性は相対パスを指定することができる
3. <a type="video/mp4">はリンク先が動画であることを示す
4. <a target="target">の属性targetはtargetを指定することでリンク先を新しいウィンドウで開く
5. 全て当てはまる
6. 該当なし
```

### Q3
#### 正しいものを選択してください
```css
1. idは３文字以下だと効かない
2. idの重複はCSSに影響を出す場合がありJqueryで影響は出さない
3. idの重複はコーディング規約で違反とされている
4. inputでidをつける場合、nameと同じにしなくてはならない
5. 全て当てはまる
6. 該当なし
```

### Q4
#### 正しいものを選択してください
```html
<p class="p1">アイウエオ</p>
<h4 class="h4">カキクケコ</h4>
<div class="div1">
    <p class="p2">
      サシスセソ
        <span class="span1">タチツテト</span>
    </p>
    <p class="p3">
      ナニヌネノ
        <span class="span2">
            ハヒフへホ
        </span>
    </p>
</div>
<p class="p4">マミムメモ</p>
```
```css
h4 ~ p {
  color:red;
}
div > p{
    color: blue;
}
```
```
1. クラスp1は青文字になる
2. span1,span2は赤文字になる
3. クラスp2,p3のみ青文字になる
4. クラスp4は赤文字になる
5. 全て当てはまる
6. 該当なし
```
### Q5
#### 正しいものを選択してください
画像１  
<img width="244" alt="スクリーンショット 2020-04-22 18 26 52" src="https://user-images.githubusercontent.com/48113599/79965506-10985b00-84c7-11ea-93c0-5e76e055649e.png">  
画像２  
<img width="275" alt="スクリーンショット 2020-04-22 18 26 45" src="https://user-images.githubusercontent.com/48113599/79965498-0c6c3d80-84c7-11ea-9751-442c67c93a3c.png">  
画像１を画像２に変える場合正しいCSSはどれか  
```css
1. 
div.box1{
    width: 200px;
    background-color: red;
}
div.box2{
    width: 200px;
    background-color: blue;
    margin: 10px;
    padding: 10px 0px;
}
2. 
div.box1{
    width: 200px;
    background-color: red;
}
div.box2{
    width: 200px;
    background-color: blue;
    margin-top: 10px;
    padding: 10px 10px;
}
3. 
div.box1{
    width: 200px;
    background-color: red;
}
div.box2{
    width: 200px;
    background-color: blue;
    margin: 10px 0px;
    padding: 10px;
}
4. 
div.box1{
    width: 200px;
    background-color: red;
}
div.box2{
    width: 200px;
    background-color: blue;
    margin: 10px 0px;
    padding: 10px 0px;
}
6. 全て当てはまる

5. 該当なし
```
### Q6
#### 正しいものを選択してください
画像３  
<img width="405" alt="スクリーンショット 2020-04-22 18 49 59" src="https://user-images.githubusercontent.com/48113599/79967732-2e1af400-84ca-11ea-8014-d3001d6da833.png">  
画像４  
<img width="401" alt="スクリーンショット 2020-04-22 18 49 40" src="https://user-images.githubusercontent.com/48113599/79967735-2fe4b780-84ca-11ea-8956-a166553d2899.png">  
- 画像3から画像４に変更させるために必要なflexboxの要素を正しく記述しているものを選んでください  
- ※文字色や全体のwidth,hright、ボックス内のCSSは無視して良いとする  
```html
<div class="flex">
    <div class="f1">
        1
    </div>
    <div class="f2">
        2
    </div>
     <div class="f1">
        3
    </div>
    <div class="f2">
        4
    </div>
     <div class="f1">
        5
    </div>
    <div class="f2">
        6
    </div>
</div>
```
```css
1. 
.flex{
    display: flex;
    justify-content: space-around;
    flex-direction: row;
}
2. 
.flex{
    display: flex;
    justify-content: space-around;
    flex-flow: wrap;
}
3.
.flex{
    display: flex;
    flex-wrap: wrap-reverse;
    justify-content: center;
}
4.
.flex{
    display: flex;
    flex-wrap: wrap;
    align-items: center;
}

5. 全て当てはまる
6. 該当なし

```
### Q7
#### 擬似要素 :before,:afterについて正しいものを選択してください

```html
<h3 class="question7">擬似要素について</h3>
```
```css
.question7::【○○○】{
    content: "test";
    color: skyblue;
}
```
<img width="235" alt="スクリーンショット 2020-04-22 19 25 51" src="https://user-images.githubusercontent.com/48113599/79971316-198d2a80-84cf-11ea-82fb-7082516a1f7f.png">  
画像をみて選択してください  

```css
1. ○○○に入るにはafter 擬似要素はSEOに影響する
2. ○○○に入るにはbefore 擬似要素はSEOに影響する
3. ○○○に入るにはafter 擬似要素はSEOに影響しない
4. ○○○に入るにはbefore 擬似要素はSEOに影響しない
5.全て当てはまる
6.該当なし
```

### Q8
#### 正しいものを選んでください

画像５  
<img width="491" alt="スクリーンショット 2020-04-22 19 47 18" src="https://user-images.githubusercontent.com/48113599/79973193-147daa80-84d2-11ea-82a4-f02218014a1f.png">   
画像6  
<img width="479" alt="スクリーンショット 2020-04-22 19 45 38" src="https://user-images.githubusercontent.com/48113599/79973069-df715800-84d1-11ea-8b40-243e00dc2466.png">  

画像５を画像６にする際に正しいCSSの記述を選択してください  
```html
<div class="question8">
    div1
    <div class="div2">div2 </div>
</div>
```
```css
1.
.question8{
    background-color: skyblue;
    height: 80px;
    width: 30%;
    position: relative;
}
.question8 > div{
    background-color: white;
    padding: 5px;
    margin: 3px;
    position: absolute;
    bottom: 0px;
    right: 0px;
}
2.
.question8{
    background-color: skyblue;
    height: 80px;
    width: 30%;
    position: relative;
}
.question8 > div{
    background-color: white;
    padding: 5px;
    margin: 3px;
    position: absolute;
    top: 0px;
    right: 0px;
}
3.
.question8{
    background-color: skyblue;
    height: 80px;
    width: 30%;
    position: absolute;
}
.question8 > div{
    background-color: white;
    padding: 5px;
    margin: 3px;
    position: relative;
    bottom: 0px;
    left: 0px;
}
4.
.question8{
    background-color: skyblue;
    height: 80px;
    width: 30%;
    position: absolute;
}
.question8 > div{
    background-color: white;
    padding: 5px;
    margin: 3px;
    position: relative;
    top: 0px;
    right: 0px;
}
5.全て当てはまる

6.該当なし
```

### Q9
#### 正しいものを選択してください
画像７  
<img width="71" alt="スクリーンショット 2020-04-22 19 56 48" src="https://user-images.githubusercontent.com/48113599/79973963-6a9f1d80-84d3-11ea-8c26-d83c569738ac.png">  
画像８  
<img width="77" alt="スクリーンショット 2020-04-22 19 56 30" src="https://user-images.githubusercontent.com/48113599/79973967-6bd04a80-84d3-11ea-93ab-f567e91027d3.png">  
画像7を画像８にする際に使用するCSSはどれか  
```css
1. border-circle
2. radius
3. border-radius
4. align-items
5.全て当てはまる
6.該当なし
```

### Q10
#### 正しいものを選択してください
ある画像Aを画像Bの枠にマスクしたいときに正しいCSSを選択してください 

- マスク対象の画像A　./img/flower.jpg  
![flower](https://user-images.githubusercontent.com/48113599/79977846-e734fa80-84d9-11ea-8aa5-42c1d0ba48d1.jpg)  

- マスクに使用する画像B　./img/star.png'  
![star](https://user-images.githubusercontent.com/48113599/79977845-e56b3700-84d9-11ea-94be-b8a3ebbd575f.png)  

- 完成イメージ  
![demo3](https://user-images.githubusercontent.com/48113599/79978047-3844ee80-84da-11ea-8aa7-b8c37cc8ff5b.jpg)  

```html
<!-- 花の画像　パスは気にしないものとする -->
<div class="item">
  <img src="./img/flower.jpg" alt="花" class="background">
</div>
```
```css
1.
.item {
  -webkit-mask-image: url('../img/star.png');
  mask-image: url('../img/star.png');

}
３.
.item {
  -webkit-mask-image: url('../img/star.png');
  mask-image: url('../img/star.png');
  mask-repeat: no-repeat;
  -webkit-mask-position: center;
  mask-position: center;
}
３.
.item :after{
  -webkit-mask-image: url('../img/star.png');
  mask-image: url('../img/star.png');
  mask-repeat: no-repeat;
  -webkit-mask-position: center;
  mask-position: center;
}
4.
.item:before {
  -webkit-mask: append('../img/star.png');
  mask: append('../img/star.png');
}
5.全て当てはまる

6.該当なし
```

