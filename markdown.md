# Markdown記法チートシート
## Format Text - テキストの装飾

### Headers - 見出し

* \# これはH1タグです
* \## これはH2タグです
* \###### これはH6タグです

### Emphasis - 強調

* \*これはイタリック体です*
* \_これもイタリック体です_
* _これは_イタリック体になりません
* \*\*これは太字です**
* \_\_これも太字です__

## Lists - リスト

### 順序なしリスト

* 文頭に「*」「+」「-」のいずれかを入れると順序なしリストになります
* 要点をまとめる際に便利です
* リストを挿入する際は、**リストの上下に空行がないと正しく表示されません**

### 順序つきリスト

1.  文頭に「数字.」を入れると順序つきリストになります
2.  1.2.3.と入れていくといい具合です
3.  リストを挿入する際は、**リストの上下に空行がないと正しく表示されません**

## Blockquotes - 引用

> \> 文頭に>を置くことで引用になります。
> \> 複数行にまたがる場合、改行のたびにこの記号を置く必要があります。
> \> **引用の上下にはリストと同じく空行がないと正しく表示されません**
> \> 引用の中に別のMarkdownを使用することも可能です。

> > これはネストされた引用です。

## Horizontal rules - 水平線

下記は全て水平線として表示されます

> \* * *
> \***
> \*****
> \- - -
> \---------------------------------------

## Links - リンク

* \[リンクテキスト](URL "タイトル") 
    * タイトル付きのリンクを投稿できます。

**例**

> *Markdown:* \[Google]\(https://www.google.co.jp/ "Google")

*結果:* [Google](https://google.co.jp "Google")

* \[リンクテキスト](URL) 
    * こちらはタイトル無しのリンクになります。

**例**

> *Markdown:* \[Google]\(https://www.google.co.jp/)

*結果:* [Google](https://google.co.jp)

## Images - 画像埋め込み

* \![代替テキスト]\(画像のURL)
    * タイトル無しの画像を埋め込む
* \![代替テキスト]\(画像のURL "画像タイトル")
    * タイトル有りの画像を埋め込む

**例**

> *Markdown:* \![拾い画]\(https://pbs.twimg.com/profile_images/378800000220029324/fe66faeca20115da8566e51d83447ead_400x400.jpeg "拾い画")

*結果:*
> ![拾い画](https://pbs.twimg.com/profile_images/378800000220029324/fe66faeca20115da8566e51d83447ead_400x400.jpeg "拾い画")

## Tables - テーブル
```
| Left align | Right align | Center align |
|:-----------|------------:|:------------:|
| This       |        This |     This     |
| column     |      column |    column    |
| will       |        will |     will     |
| be         |          be |      be      |
| left       |       right |    center    |
| aligned    |     aligned |   aligned    |
```

上記のように書くと、以下のように表示されます。

| Left align | Right align | Center align |
|:-----------|------------:|:------------:|
| This       |        This |     This     |
| column     |      column |    column    |
| will       |        will |     will     |
| be         |          be |      be      |
| left       |       right |    center    |
| aligned    |     aligned |   aligned    |

## その他

バックスラッシュ[\\]をMarkdownの前に挿入することで、Markdownをエスケープ(無効化)することができます。

**例**

> \# H1
> エスケープされています
