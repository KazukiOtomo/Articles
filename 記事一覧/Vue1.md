# Vue備忘録

## はじめに
Vue.jsで扱うUIの定義をしたいので、
HTMLファイルの中で、divを定義します。
コメントで消してある部分です。
今回、idは”sample”としています。

```html 
<!-- HTMLファイル(.html) -->

<!DOCTYPE html>
<html lang="ja">
    <head>
        <meta charset="UTF-8">
    </head>
    <body>

        <!-- <div id="sample"></div> -->

        <script src="https://cdn.~/npm/vue">
        </script>
    </body>
</html>
```

次に、javascriptファイルで格納するデータの管理を行います。
ファイルの場所に指定はありませんが、HTMLファイルからたどれるように場所を覚えておく
必要はあります。

では、Vueでモデルを作っていきます。
```js
// javascriptファイル(.js)
(function() {
  'use strict';

  
  var vm = new Vue({
    el: '#sample',　//どの領域のVueと結び付けるかelementの略のelというキーで指定する
    data: {　
      name: 'otomo'　//保持するデータを管理する
    }
  });
})();
```

これでdata->UIへの反映が完了したので、
今度は、UI->dataへの反映を行います。
（双方向バインディング）

```html
<!-- HTMLファイル（.html） -->

<!DOCTYPE html>
<html lang="ja">
    <head>
        <meta charset="UTF-8">
    </head>
    <body>
        <div id="sample">
            <!-- 「{{}}」で、javascript内のキーを指定 -->
            <p>Hello {{ name }}!</p>
            <!-- inputタグで入力を受け付け、v-modelでフォーム入力バインディングを行う -->
            <p><input type="text" v-model="name"></p>
        </div>
        <script src="https://cdn.~/npm/vue">
        </script>
    </body>
</html>
```

このHTMLファイルを実行すると、
フォームに入力された内容がリアルタイムで反映されている
様子が確認できると思います。
v-modelについての解説は
[こちら(公式ドキュメント)](https://jp.vuejs.org/v2/guide/forms.html)





