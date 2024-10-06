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

https://myst-parser.readthedocs.io/en/latest/syntax/images_and_figures.html#block-level-images

https://myst-parser.readthedocs.io/en/latest/syntax/images_and_figures.html#figures-images-with-captions

他のSphinxのディレクティブを使う場合は、以下のMyST-Parser公式ドキュメントを参照してください（たぶん、ほぼ使うことはないと思いますが）。

[Roles and Directives](https://myst-parser.readthedocs.io/en/latest/syntax/roles-and-directives.html)

## プレビューの確認方法
プルリクエストごとにRead the Docsでプレビューが見られるようになっています。プレビューURLの取得方法は以下のとおりです。

ます、以下のURLを開きます。

https://report2024.readthedocs.io/ja/latest/

以下の手順でプレビューURLを取得します。

![step1](https://github.com/user-attachments/assets/554d2bae-1d67-4670-91d7-da9548465bf1)
<img width="712" alt="step2" src="https://github.com/user-attachments/assets/4cc514ef-a967-437e-bbc5-a63bf3febb01">
![step3](https://github.com/user-attachments/assets/2667206c-7520-4dec-8b95-c67d8a3a2670)
![step4](https://github.com/user-attachments/assets/e010ef5c-58c0-4100-9eb7-804d2c1477b9)

## レビューコメントの付け方
レビューコメントには[hypothes](https://web.hypothes.is/)のアカウントが必要です。
プレビューのコメントしたい箇所を選択状態にすると、「Annotate」というメニューが表示されます。これをクリックするとコメントを付けられます。
