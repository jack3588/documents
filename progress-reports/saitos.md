# 2017/09/12

# 今月の目標
- Androidでマップ機能を表示する

# やったこと
- GoogleMapの表示
  - 新規PJ作成の際Activityの種類を「Google Maps Activity」に選択するだけで表示できた
    - 初期表示画面の設定をAndroidManifestで設定
    - 自分の発行したAPIキーをAndroidManifestで設定

- DBの実装
  - sqLiteの実装
    - Create tableの実装
    - Insertの実装
    
※selectせずにinsertだけしているので登録できているか不明。
insertした後の画面表示も整えてないので再登録もやりづらくて中途半端な状態です。

# 気付き
- Google Map表示時にエミュレーターのバージョンが合わずに表示できない場合は「app/build.gradle」でバージョン指定
- DBはテーブルがなければ作成、あれば読み込みをしてくれるらしい
- SQLiteはプロトコルやプロセス通信使わずにAPIを呼び出して動くもの

# 次回目標
- DBの仕組みをもうちょっと調べてアプリに組み込む（select、updateくらいまでやりたい）
- GoogleMapを動かす仕組み、Classも調べたい（できれば）
