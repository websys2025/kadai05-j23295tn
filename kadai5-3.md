## 外部APIの呼び出しのミニレポート
### Q3-1. 郵便番号APIについて説明せよ。
* エンドポイントと機能
* https://zipcloud.ibsnet.co.jp/api/search
* 日本郵便が公開している郵便番号データを検索する機能。郵便番号を入力すると、対応する住所情報を返す。

* リクエストとレスポンスのフォーマット
* GET https://zipcloud.ibsnet.co.jp/api/search?zipcode=2720025
* {"status": 200,"message": null,"results": {"zipcode": "2720025","prefcode": "12","address1": "千葉県","address2": "市川市","address3": "大和田","kana1": "ﾁﾊﾞｹﾝ","kana2": "ｲﾁｶﾜｼ","kana3": "ｵｵﾜﾀﾞ"}}
  
### Q3-2. 各自で調査したAPIについて説明せよ。
* APIの名称と参照URL
* Foodish API
* https://foodish-api.com/
  
* エンドポイントと機能
* https://foodish-api.com/api/
* 実行するたびに異なる料理の写真を返す機能。
  
* リクエストとレスポンスのフォーマット
* GET https://foodish-api.herokuapp.com/api
* {"image": "https://foodish-api.herokuapp.com/images/ランダムな料理の画像"}

### Q3-3. 感想
* 今回の課題で苦労したこと
* 非同期通信、async/awaitを理解するために教科書で調べたこと。
* レスポンスのフォーマットの理解。

* 演習を通して理解できたこと
* Web APIの動作のさせ方。
* 非同期処理の基本的な使い方。

* Web APIの利便性や課題など
* Web APIを使うことで、外部データを簡単に取得してページに動的に表示できる。
* 外部に依存することで通信エラーやその他の問題が起こりやすくなるため、そこが多くのAPIを使う上での課題だと感じた。

