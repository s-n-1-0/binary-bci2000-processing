# binary-bci2000-processing

https://github.com/s-n-1-0/MLA_BCI2000 から信号処理モジュールを分離してpypiパッケージにしたもの。
できればBCPy2000は使いたくないので、このパッケージの使用をやめるようにしたい。


## 仕様
次のステータスを送受信できるようにしておく必要があります。  
※しないと正常にデータが保存されない。

### 本モジュールが送信するステータス
+ `predictClass` : 予測したクラスを返す(0:None, 1:左, 2:右)
+ `predictCount` : 何回目の予測か

### 本モジュールが受信するステータス
+ `trialNum` : 何試行目か
+ `trueClass` : 目的のクラス(0,1,2)
