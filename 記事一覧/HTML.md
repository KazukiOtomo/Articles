# タグ一覧&お役立ち情報

## ページアイコンの設定
```html
<!-- 「favicon.icoを置いておくと自動で読み込まれる場合もある。」 -->
<head>
    <link rel="icon" href="favicon.ico">
</head>
```

## 引用の設定
```html
<!-- cite属性を使うことで、引用部分を示すことができる(解析専用) -->
<blockquote cite="https://sample.com">
    <p>HTMLはこれから学ぶべきスキルです！</p>
</blockquote>
```

## 画像のサイズ変更と属性追加
```html
<!-- alt属性を使うと、目が不自由な方が読み上げに使えるらしい -->
<body>
    <img src="img/logo.png" width="300" height="50" alt="これはタイトルのロゴです">
</body>
```

## リストの種類
```
・箇条書きリスト（<"ul>"）unordered list
・順序付きリスト（<"ol>”）ordered list
・説明付きリスト（<"dl>"）descliption list
```

## 便利なコマンド
```
・Alt　+　↑　↓キーで行を入れ替える
・Ctrl　+　D でマルチカーソルを使うことができる。
・
```

## 表の書き方
```html
<table>
    <thead>
      <tr>
        <th>年</th>
        <th>出来事</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>2014</td>
        <td>会社設立</td>
      </tr>
      <tr>
        <td>2016</td>
        <td>サイトリニューアル</td>
      </tr>
    </tbody>
  </table>
```

## ページ内リンクの作り方
```html
<p><a href="#target">ページ内の飛ばしたい場所へ</a>
</p>

//処理

<!-- ページ内のこの場所まで飛んでくる -->
<p id="target"></p>


<a href="#top">ページの先頭まで飛ぶ</a>
```

## 入力タグinput
```html
<!-- 目の不自由な方が使う読み上げ機能は、このlabelタグを読み込むらしい -->
<label>名前 <input type="text">
</label>
```

## 面白そうなinputタグ
```html
<!-- ※総じて、ブラウザによってサポートされていない場合があるので注意 -->
<body>

<!-- 色を選択するカラーPickerが出てくる -->
  <p><input type="color"></p>

<!-- カレンダーが出現して、日時を選択できる -->
  <p><input type="date"></p>

  <!-- 数値のみを入力受付するようにできる -->
  <p><input type="number"></p>
  
  <!-- スライダーが出現して、値を入力できる -->
  <p><input type="range"></p>
  
</body>
```



## 役に立ちそうなタグ一覧
<img src=image.jpg>




