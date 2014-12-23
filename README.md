# non-carbo

糖質ゼロ、低炭水化物食品データベースサイト。(non carbohydrate)

## 必要環境

- ruby2.1.5
- rails4.2

## インストール

```bash
$ brew install imagemagick postgresql qt chromedriver
$ createuser -s non_carbo
$ git clone git@github.com:komagata/non_carbo.git
$ cd non_carbo
$ bundle
$ rake db:setup
$ rails s
$ open http://localhost:3000
```

## テスト

    $ rake test:all

seleniumを使ってのテスト

    $ USE_SELENIUM=TRUE rake test:all

## デプロイ

    $ rake production deploy
    $ rake staging deploy
