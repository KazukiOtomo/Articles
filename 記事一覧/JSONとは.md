# JSONとは
JSONは、「JavaScript Object Notation」の略で、<br>
要は、JavaScriptを元にしたデータ定義方法のこと。<br>

## JSONの特徴
・PythonやJava、PHPなどの幅広い言語で使える。<br>
・クライアント言語とサーバサイド言語間のデータのやり取りに使われる。<br>

<br>
<span style="color: blue; ">

*クライアント言語：JavaScriptやCSS等のようなWebサーバーから結果がブラウザに返ってきてブラウザ側で処理をする時に動作する言語。フロントエンドで使われている技術のこと。*

</span>

<br>

<span style="color:blue;">

*サーバサイド言語：JavaやPythonといった、サーバ側で動く言語のこと。<br>
ちなみに、クライアント言語と違って、ユーザ側から見ることができない。*

</span>

## JSONとXMLの違い
データのやり取りをするにあたって、XMLというものもあります。<br>
これは、JSONが登場する前から使われていたもので、<br>
HTMLの記法が元になっています。<br>
それぞれの言語で同じことをするプログラムを書いて比較すると...

**XMLでの記法**
```
<?xml version="1.0"encording="utf-8"?>
<data>
 <item>
   <id>1</id>
   <name>suzuki</name>
 </item>
 <item>
  <id>2</id>
  <name>satou</name>
 </item>
</data>
```

**JSONでの記法**
```
[
    {"id":"1","name":"suzuki"},
    {"id":"2","name":"satou"}
]