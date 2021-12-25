SchemaSpy : DB内部データの自動可視化処理
==
~~~
Date   : 2021.12.25
Author : Yugeta.Koji
~~~

# Summary
- 既存のデータベースのER図や、テーブル一覧資料を自動で作成してくれる"SchemaSpy"をDockerで便利に利用できる処理一式を格納しています。


# Run
- Dockerを起動した状態で下記をコマンドを実行してください。
$ sh run.sh




--- old:

# Summary
- データベースのテーブル数が200以上あり、構成図などが存在しないとの事だったので、ER図や、それぞれのDB,テーブル情報を自動作成し、ER図まで作ってくれる"SchemaSpy"というシステムをdockerで便利に利用できることがわかったので、実行して現段階（2021.12.23現在）の構成図を作成してみた。
- 

# 作成環境
- MacBookAir 2020 M1


# 実行
- このディレクトリ構成をDL(clone)して、docker-compose.ymlのある階層で、以下コマンドを実行すると、outputフォルダが作られて、数分でファイルが作成完了します。
- $ docker-compose up


# 以下参考情報
- schemasqlについて
  - url : https://hub.docker.com/r/schemaspy/schemaspy/
  - $ docker run -v "$PWD:/output" -v "[path-to-config-file]:/nadia.properties" schemaspy/schemaspy:[snapshot, latest or specific version] [options]

- PostgreSQL ドライバダウンロードサイト
  - 参考 : https://tyoshikawa1106.hatenablog.com/entry/2016/09/09/213438
  - url : https://jdbc.postgresql.org/download.html
