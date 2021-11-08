- プライベートリポジトリ(https://github.com/mono0926/Sesame-Private)から最低限仕上げて移植予定
  - https://twitter.com/_mono/status/1455733207198945281

# SesameUnlocker

- Apple WatchのComplicationボタンをタップされたら、[kishikawakatsumi/Doorlock](https://github.com/kishikawakatsumi/Doorlock)の[`unlock()`処理](https://github.com/kishikawakatsumi/Doorlock/blob/main/Doorlock/Device.swift#L9)が即座に呼ばれる
- 解錠に特化していて、それ以外の操作・表示は公式アプリなど使えば良いという考え
  - ただし、電池切れはクリティカルなのでComplicationボタンをタップ後に表示される画面でその表示および残量低下時には毎回ローカル通知発行する
