# C#基本文法まとめ

**本記事は、Unityを扱うにあたって、知っておくべき
基本的な文法についてまとめたものです**

## **bool型**
 
```csharp
;bool型変数には、「true」か「false」しか入れない。
;Javaでのboolean型と同じ
bool example = true;
```
 
 

## **int型　float型**
 
```cs
//int型変数には、大体-21憶から21億までの整数が格納される。
//この範囲を超える整数は、long型で扱うことができる。
int example = 64;
 
 
//小数を格納することができる。
//数値の末尾に「f」をつけることで、float型であることを表す
//誤差が許容される有効桁数は、６～９桁
float example = 3.2f;
```
 
## **string型**     

~~//JavaではStringだが、C#ではstringなので注意~~

**→C#では、Stringでもstringでも文字列を扱うことができる**

```csharp
//string型では、文字列を格納できる。    
string example = "文字列";
```

 
 
## **配列型**

 ```cs
    //配列の宣言
    int arrays [] = new int [] {1,2,3}; 
 
    //配列の長さ(大きさ)をコンソールに表示する。ここでは、「３」と表示される。
    Debug.Log(arrays.length); 
 
    //配列の番号を指定してコンソールに表示する。ここでは、「１」と表示される。
    Debug.Log(arrays[0]); 
 
 
    //配列の番号を指定して、内容を書き換える。
    arrays[0] = 900;
 
    //書き換えた内容の表示。ここでは、「900」と表示される。
    Debug.Log(arrays[0]);
```
 
## **List型**
 
```cs
    //配列型は、最初に宣言した個数までの要素番号しか使えないが、
    //List型では、後から追加していくことができる。
    List <int> lists = new List <int> {1,2,3};
 
    //listsの中の個数をカウントする。ここでは、「3」と表示される。
    Debug.Log(lists.Count);
 
    //List型listsに「800」のデータを追加する。
    lists.add(800);
 
    //さっき追加したデータが、末尾に入っていることを確認する。
    //ここでは、「800」と表示される。
    Debug.Log(lists[3]);

```
 
## **Dictionary型**

```cs
    //List型と異なるのは、値を取り出す際に指定した文字列を使うことができる点。
        Dictionary <String,int> values = new Dictionary <String,int>{
            {"ひっかく",30},
            {"たいあたり",40},
            {"つつく",35},
        };
 
     //「ひっかく」の威力が100に変更される（チートです！）
     values["ひっかく"] = 100;
 
      //威力30の「ひのこ」が追加される。
      values.add("ひのこ",30);
 
```
 
 
 
 
## **列挙型**

```cs
    //enum型は、値の種類を先に宣言しておくことができる
    //ここでは、Easy,Normal,Difficultの3つしか入れることができなくなっている。
    enum GAMEMODE{
        Easy,
        Normal,
        Difficult
    }
 
    GAMEMODE gamemode = GAMEMODE.Easy;
 ```
 
## **定数**

```cs
    //constを付けると、その値は変更できなくなる。
    //Javaでのfinalと同じ
    const int example = 10;
 ```
 
## **ベクトル型**

```cs
        //varは型推論といって、勝手に型を補ってくれる。
        var position = new Vector3(0, 1, 2);
 
        //座標を(0,1,2)に移動させる。
        transform.position = position;
 
        //ベクトル同士の演算も可能。結果は、(2, 4, 6)
        Debug.Log(new Vector3(0, 1, 2) + new Vector3(2, 3, 4));
 ```
