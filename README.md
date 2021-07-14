# sample-ajax
授業中のリソースの置き場所

ajax の get を行う為のテンプレート
## jQuery 側の json オブジェクトの準備
```javascript
formData = {};
```
{} は 空の json オブジェクト
```javascript
formData["param1"] = "テスト";
```
formData のプロパティは formData["プロパティ文字列"] に値をセットして作成される

formData のプロパティは formData.プロパティ文字列 と書く事もできます
```javascript
formData.param1 = "テスト";
```
## jQuery 側からサーバへデータを送る
```javascript
data: formData
```
```javascript
{
	"param1": "テスト"
}
```
http://localhost/app/form-action-json.php?param1=%E3%83%86%E3%82%B9%E3%83%88&_=1626243759099

と言うフォーマットに jQuery に加工されてサーバの PHP が呼び出されます
## PHP でデータを受け取る
QuertyString と呼ばれる ? 以降の文字列が $_GET にセットされて PHP に入る
```javascript
param1=%E3%83%86%E3%82%B9%E3%83%88&_=1626243759099
```
$_GET["param1"] に "テスト" がセットされて スーパーグローバル変数として利用可能となる。


