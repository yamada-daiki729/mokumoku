# README

## 環境構築
```
$ bundle install
$ bin/rails db:setup
$ yarn install
$ bin/rails s
```

## 事業をエンジニアリングしよう提案編の回答は以下に記述してください
選択した事業側の課題
サービス登録者数の内、男性60%に対して、女性は40%。一方で、サービス内のもくもく会に参加した人の比率は、男性90%：女性10%と大きな差が出ています。もっと女性が使いやすいようなサービス設計にする必要があるのではないか？
提案内容
現状ユーザー情報に性別がなく、もくもく会参加者の男女比率が全くわからない状態である。
周りが男性しかいないかもしれないと、女性は参加するのに躊躇してしまっていると推測する。
なのでもくもく会一覧のボード中に男女比率を表示する。
もくもく会作成時に、男性限定、女性限定の条件を追加できるようにする。

実装方針
・ユーザーに性別カラムを追加する。
・もくもく会の中の参加者nameの横に性別マークを入れる。
・ボード一覧画面と、詳細画面に男女比率を記載する
・もくもく会作成時に指定なし、男性限定、女性限定のセレクトを用意する。
・男性限定or女性限定の条件付きもくもく会には、異性は参加ボタンを表示しないようにする
