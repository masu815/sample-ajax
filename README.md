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
