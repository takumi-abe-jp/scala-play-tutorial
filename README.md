## 概要
- scala
- play framework v2.8.x

実行コマンド

```bash
$ sbt new playframework/play-scala-seed.g8
```

play appの構造
(このprojectはappをtestで作成)

```bash
app                      → アプリケーションソース
 └ assets                → コンパイルされたアセットソース
    └ stylesheets        → 通常は LESS CSS ソース
    └ javascripts        → 通常は CoffeeScript ソース
 └ controllers           → アプリケーションコントローラ
 └ models                → アプリケーションビジネス層
 └ views                 → テンプレート
build.sbt                → アプリケーションビルドスクリプト
conf                     → 設定ファイル、および (クラスパス上の) その他のコンパイルされないリソース
 └ application.conf      → メイン設定ファイル
 └ routes                → ルート定義
dist                     → プロジェクト成果物に含める任意のファイル
public                   → 公開アセット
 └ stylesheets           → CSS ファイル
 └ javascripts           → Javascript ファイル
 └ images                → 画像ファイル
project                  → sbt 設定ファイル群
 └ build.properties      → sbt プロジェクトの目印
 └ plugins.sbt           → Play 自身の定義を含む sbt プラグイン
lib                      → 管理されていない依存ライブラリ
logs                     → ログフォルダ
 └ application.log       → デフォルトログファイル
target                   → 生成物
 └ resolution-cache      → 依存性に関する情報
 └ scala-2.10
    └ api                → 生成された API ドキュメント
    └ classes            → コンパイルされたクラスファイル
    └ routes             → routes から生成されたソース
    └ twirl              → テンプレートから生成されたソース
 └ universal             → アプリケーションパッケーｓ時
 └ web                   → コンパイルされた web アセット
test                     → 単体、および機能テスト用のソースフォルダ
```


## 参考
- https://www.playframework.com/documentation/2.8.x/Home
- https://scala-text.github.io/scala_text/