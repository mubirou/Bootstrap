# Bootstrap
Bootstrap 5 超入門ノート

### <b>INDEX</b>

|No.|内容|No.|内容|
|:--:|:--|:--|:--|
|001|[Bootstrap について](#aboutBootstrap)|002|[ボタン](#button)|
|003|[ボタングループ](#buttonGroup)|004|[XXXXXXXXX](#)|
|005|[XXXXXXXXX](#)|006|[XXXXXXXXX](#)|
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



<a name="buttonGroup"></a>
# 003 <b>ボタングループ</b>

参考：https://getbootstrap.jp/docs/5.0/components/button-group/

### ラジオボタングループ
これが一番使いやすそう
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
        <div class="btn-group" role="group" aria-label="Basic radio toggle button group">
            <input type="radio" class="btn-check" name="btnradio-A" id="btnradio-1" autocomplete="off">
            <label class="btn btn-outline-danger" for="btnradio-1">選択１</label>
          
            <input type="radio" class="btn-check" name="btnradio-A" id="btnradio-2" autocomplete="off">
            <label class="btn btn-outline-danger" for="btnradio-2">選択２</label>
          
            <input type="radio" class="btn-check" name="btnradio-A" id="btnradio-3" autocomplete="off">
            <label class="btn btn-outline-danger" for="btnradio-3">選択３</label>
        </div>
    </body>
</html>
```

デフォルトで何れかを選択しておきたい場合は最後に checked を追加する（記述例）
```
<input type="radio" class="btn-check" name="btnradio" id="btnradio1" autocomplete="off" checked>
```

サンプルは[こちら](https://mubirou.github.io/Bootstrap/examples/html/003.html)

実行環境：Bootstrap 5.0.1、Google Chrome 90、Windows 10、Visual Studio Code  
作成者：夢寐郎  
作成日：2021年05月27日  



<a name="form"></a>
# 004 <b>フォーム</b>

参考：https://getbootstrap.jp/docs/5.0/forms/overview/

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
        <form style="max-width: 480px; margin: auto;">
            <div class="mb-3">
                <label for="name1" class="form-label">お名前（必須）</label>
                <input class="form-control" id="name1" type="text" placeholder="例：鈴木太郎">
            </div>
            <div class="mb-3">
                <label for="email1" class="form-label">e-mail（必須）</label>
                <input type="email" class="form-control" id="email1" placeholder="例：example@gmail.com">
            </div>
            <div class="mb-3">
                <label for="age1" class="form-label">年齢（オプション）</label>
                <select class="form-select" id="age1">
                    <option selected>選択してください</option>
                    <option value="20歳未満">20歳未満</option>
                    <option value="20-29歳">20-29歳</option>
                    <option value="30-39歳">30-39歳</option>
                    <option value="40-49歳">40-49歳</option>
                    <option value="50-59歳">50-59歳</option>
                    <option value="60-69歳">60-69歳</option>
                    <option value="70-79歳">70-79歳</option>
                    <option value="80歳以上">80歳以上</option>
                </select>
            </div>
            <div class="mb-3">
                <label for="sex1" class="form-label">性別（オプション）</label>
                <div class="form-check">
                    <input class="form-check-input" type="radio" name="flexRadioDefault" id="sex1">
                    <label class="form-check-label" for="sex1">
                        男
                    </label>
                </div>
                <div class="form-check">
                    <input class="form-check-input" type="radio" name="flexRadioDefault" id="sex1">
                    <label class="form-check-label" for="sex1">
                        女
                    </label>
                </div>
                <div class="form-check">
                    <input class="form-check-input" type="radio" name="flexRadioDefault" id="sex1">
                    <label class="form-check-label" for="sex1">
                        その他
                    </label>
                </div>
            </div>
            <div class="mb-3">
                <label for="textarea1" class="form-label">備考欄（オプション）</label>
                <textarea class="form-control" id="textarea1" rows="3" placeholder="ご不明な点ございましたらお書き下さい。"></textarea>
              </div>
            <button type="submit" class="btn btn-primary">送信</button>
          </form>
    </body>
</html>
```

サンプルは[こちら](https://mubirou.github.io/Bootstrap/examples/html/004.html)

実行環境：Bootstrap 5.0.1、Google Chrome 90、Ubuntu 20.04、Visual Studio Code  
作成者：夢寐郎  
作成日：2021年05月27日  



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