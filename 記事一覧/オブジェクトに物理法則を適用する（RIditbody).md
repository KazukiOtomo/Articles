#オブジェクトに物理法則を付与するの

##Riditbodyの作成

**物理演算を付与したいゲームオブジェクトを選択し、
Component->Rigitbody->Physics->Riditbodyを選択する**

![image.png](https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/850380/548e6774-cdc2-425a-d0cc-ee981220e83d.png)

##Riditbodyの詳細解説

**Riditbodyの要素を、以下にまとめておく。**

![image.png](https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/850380/d66b9369-3ae5-066d-e29e-7be3f4cbe0f6.png)


|名前 |詳細|
|-----|-----------------|
|Mass |オブジェクトの重さ(重さはkg)|
|Drag |空気抵抗の大きさ。<br>大きくするとオブジェクトが動きにくくなる|
|Angular Drag|回転に対する空気抵抗|
|Use Gravity|重力を適用するかどうか選択する|
|Is Kinematic|建物や壁に使用する。<br>スクリプトで動かさない限り動かないようになる。|
|Interpolate|これをONにするとスムーズな映像になるが、<br>あまり使いすぎると重くなりすぎるので注意|
|Collision Detection|オブジェクトを高速移動させたとき、壁などを貫通することがあるが、これをONにすると防ぐことができる。|
|Constraints|各座標軸に対して、Freeze Positionで移動、Freeze Rotationで<br>回転しないようにすることができる