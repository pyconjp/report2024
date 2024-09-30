# PyCon JP 2024開催後レポート原稿

gihyo.jpに載せるPyCon JP 2024開催後レポートの原稿です。

関連するJIRAチケットのリンク: https://pyconjp.atlassian.net/browse/TAT-668

## 環境構築方法
Python 3.9以上が必要です。

```bash
$ python -m venv env
$ source env/bin/activate
$ pip install -r requirements.txt
$ make html
$ ls build/html  # ここにHTMLファイルが生成されます
01-preface       05-talk-english  09-end           genindex.html    searchindex.js
02-keynote-day1  06-postersession 10-authors       index.html
03-keynote-day2  07-coffeebreak   _sources         objects.inv
04-talk-japanese 08-afterparty    _static          search.html
```

## 原稿の書き方
原稿はSphinxにMyST-Parserという拡張を導入して、Markdownで書けるようにしています。

画像を挿入する場合の[figureディレクティブ](https://sphinx-users.jp/reverse-dict/images/caption.html)の書き方は以下の通りです。

```markdown
```{figure} sample.jpg
:width: 600

画像のキャプション
```
```

画像のパスは、相対パスで指定してください。
`:width:`は画像の幅を指定するオプションです。指定しない場合は、元画像のサイズがそのまま使われます。

他のSphinxのディレクティブを使う場合は、以下のMyST-Parser公式ドキュメントを参照してください（たぶん、ほぼ使うことはないと思いますが）。

[Roles and Directives](https://myst-parser.readthedocs.io/en/latest/syntax/roles-and-directives.html)

## 写真の場所
以下のGoogle Driveフォルダにカメラマンが撮影した写真があります。適宜利用してください。

https://drive.google.com/drive/u/0/folders/10jx6o7viOh9zsayOX_Zbi9XJhYEZXjVf

自分で撮った写真でもOKです。

**なお、登壇者の写真を載せる場合は、本人が写真撮影に同意しているか必ず確認してください。**
