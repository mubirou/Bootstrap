# Bootstrap
Bootstrap 5 超入門ノート

### <b>INDEX</b>

|No.|内容|No.|内容|
|:--:|:--|:--|:--|
|001|[Bootstrap について](#aboutBootstrap)|002|[ボタン](#button)|
|003|[XXXXXXXXX](#)|004|[XXXXXXXXX](#)|
#

<a name="aboutBootstrap"></a>
# 001 <b>Bootstrap について</b>

### 特徴
1. HTML / CSS / JavaScript から構成されるフレームワーク
1. レシポンシブ Web デザイン対応
1. Twitter 社が開発（2011年からオープンソース化）
1. バージョン「<b>5</b>」の特徴
    * jQuery は未使用
    * バニラ JavaScript（ネイティブ JavaScript）支持
    * IE10、IE11 は未サポート
    * 2021年5月11日正式版リリース

### 開発環境の構築
1. https://getbootstrap.com/ にアクセス
1. [Download] ボタンを選択
1. [Compiled CSS and JS] の [Download] を選択
1. "bootstrap-5.0.1-dist.zip" をダウンロード
1. "bootstrap-5.0.1-dist.zip" を展開
1. "bootstrap-5.0.1-dist" フォルダ内の CSS と js フォルダを確認

### サンプル作成
1. Visual Studio Code を起動
1. 任意のフォルダに index.html を作成
1. index.html と同じ階層に上記でダウンロードした css と js フォルダをコピー
1. index.html を記述
    ```
    <!DOCTYPE html>
    <html lang="ja">
    <head>
        <meta charset="UTF-8">
        <title>xxx</title>
        <meta name="viewport" content="width=device-width,initial-scale=1.0">
        <link rel="stylesheet" href="css/bootstrap.css">
        <script src="js/bootstrap.js"></script>
    </head>
    <body>
        <h1>Hello,world!</h1>
    </body>
    </html>
    ```
1. 結果は[こちら](https://mubirou.github.io/Bootstrap/examples/html/001.html)

実行環境：Bootstrap 5.0.1、Google Chrome 90、Windows 10、Visual Studio Code  
作成者：夢寐郎  
作成日：2021年05月24日  


<a name="button"></a>
# 002 <b>ボタン</b>

参照：https://getbootstrap.jp/docs/5.0/components/buttons/

### ボタンの種類
1. ８色＋リンクボタン
1. <a><input>要素での利用
1. アウトラインボタン
1. ボタンのサイズ（大中小）
1. 非アクティブボタン
1. 全幅ブロックボタン
1. トグルボタン

### サンプルコード
```
<!DOCTYPE html>
<html lang="ja">
    <head>
        <meta charset="UTF-8">
        <title>xxx</title>
        <meta name="viewport" content="width=device-width,initial-scale=1.0">
        <link rel="stylesheet" href="../css/bootstrap.css">
        <script src="../js/bootstrap.js"></script>
    </head>
    <body>
        <button type="button" class="btn btn-primary">PRIMARY</button>
    </body>
</html>
```
サンプルは[こちら](https://mubirou.github.io/Bootstrap/examples/html/002.html)

実行環境：Bootstrap 5.0.1、Google Chrome 90、Windows 10、Visual Studio Code  
作成者：夢寐郎  
作成日：2021年05月25日  



<a name="XXXXX"></a>
# 00X <b>XXXXX</b>

### XXXXX
1. XXXX
1. XXXX
    * XXXX

### XXX
```
XXXX
```

実行環境：Bootstrap 5.0.1、Google Chrome 90、Windows 10、Visual Studio Code  
作成者：夢寐郎  
作成日：2021年0X月XX日  


© 2021 夢寐郎