# 2017/08/02

やったこと

#### メモ
・TestApp001(ボタンで切り替わるやつ)

・Calculate(電卓)

・TestApp002(画面遷移)　

### AndroidManifest.xml
```
        <activity android:name=".MainActivity">
            <intent-filter>
                <action android:name="android.intent.action.MAIN" />

                <category android:name="android.intent.category.LAUNCHER" />
            </intent-filter>
        </activity>
```

activity　アプリ内で動作してるアクティビティ（画面）

action android:name="省略" メイン画面

category android:name="省略"

このActivity（画面）を立ち上げる為のアイコンをアプリ一覧の中に表示しますーって意味

参考URL：http://nobuo-create.net/manifest/

⇒Androidstudioでactivity作ったら勝手に登録されてた

と思ってコピペしてたらActivityNotFoundExceptionで落ちた

## 画面遷移
### Intent
Activityをクラス名で指定して呼び出す方法を明示的Intent

動作(振る舞い)で呼び出し、Activityは指定しない方法を暗黙的Intent

(Gmailとかメモ帳とか他のアプリ？）

参考URL：https://techbooster.org/android/application/294/

#### 受け渡し方法
startActivityForResult(Intent, int)

遷移先からデータを受け取りたい場合に呼び出す方法

　
onActivityResult(int, int, Intent)

データを受け取る方法

startActivityだとデータを遷移元画面に戻せない


## デザイン
### 一括設定
#### res/drawable/以下にxmlファイルを設定
以下で取り込み
```
android:background="@drawable/button_background"/>
```

#### res/valuesいかにxmlファイルを設定
colors.xml
```
<color name="colorAccent">#FF4081</color>
```

style.xml
```
<item name="colorAccent">@color/colorAccent</item>
```
