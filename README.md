# my-portfolio

##コンテナの起動
wsl コンソールにてワークスペースのカレントディレクトリに移動した後、以下のコマンドを入力します。

```sh
#start
$ docker run -dit --rm --name portfolio1 -v "$PWD/public":/usr/local/apache2/htdocs/ -p 3000:80 httpd:2.4-alpine
```

##アクセス
起動後以下の URL にアクセスするとページが開けます。

<http://localhost:3000/>

##コンテナの停止
コンピュータをシャットダウンする際や、制作を終了する際は、コンテナを終了しておきます。
wsl コンソールにてワークスペースのカレントディレクトリに移動した後、以下のコマンドを入力します。

```sh
#stop
$ docker stop portfolio1
```
