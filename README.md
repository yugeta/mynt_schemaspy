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
- $ sh run.sh



# 参考
- schemasqlについて
  - url : https://hub.docker.com/r/schemaspy/schemaspy/
  - $ docker run -v "$PWD:/output" -v "[path-to-config-file]:/nadia.properties" schemaspy/schemaspy:[snapshot, latest or specific version] [options]

- PostgreSQL ドライバダウンロードサイト
  - 参考 : https://tyoshikawa1106.hatenablog.com/entry/2016/09/09/213438
  - url : https://jdbc.postgresql.org/download.html
