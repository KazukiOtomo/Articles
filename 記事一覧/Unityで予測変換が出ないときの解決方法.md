unityでVisual Studioは開くが、予測変換が出てこないという人向けの記事です。

## ①ダウンロードの確認

**まず、Visual StudioにUnityのアセンブラが入っているか確認します**

<br>

![Unityの予測変換が出ない　ver1](https://user-images.githubusercontent.com/67196994/111075513-a5ff6c00-852b-11eb-90a4-df5ececc734e.jpg)

**Visual Studioを起動すると、上記の画面になるので、**
**「新しいプロジェクトの続行」を押します。**

<br>

![Unityの予測変換が出ない　ver2](https://user-images.githubusercontent.com/67196994/111075720-b06e3580-852c-11eb-82a0-0b663cf83f97.jpg)

**すると、上のような画面になり、右側のリストの下の方にある
「さらにツールと機能をインストールする」を押します。**

![image.png](https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/850380/3ce37501-85bd-7fcf-de54-bce83a5e9eb0.png)

**Visual Studio Installerが開くので、「変更」を押します。**

![image.png](https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/850380/b0d3deed-e267-2f23-a7b5-e1dc42060140.png)

**タブが開くので、下の方へ行き、このUnityのマークがあるボックスへチェックを
入れて、ダウンロードします。
（すでにチェックがついている場合は、すでにダウンロードできているので、
　次の手順へ進みましょう）**

## ②Unity側で開くアプリの設定

**次に、Unity側の設定を行います。
デフォルトでは間違ったアプリを開くので、気を付けましょう。**

![image.png](https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/850380/a626d1ce-e614-7ab9-e1f1-da933a42a6f2.png)

**Unityを起動し、「Edit」->「Preferences」を選択します。**

![image.png](https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/850380/26832ac3-0b77-61d2-62e7-96ec4fc07c14.png)

**このようなタブが開くので、「External Tools」を選択し、
一番上のプルダウンの項目を、Visual Studio に変更すると、
予測変換が出るようになります。**

（**デフォルトでは、Open by Extensionになっています**）


以上で設定は終了です。
お疲れさまでした！
