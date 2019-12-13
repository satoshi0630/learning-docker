# learning-docker: Dockerの練習

## ミニレポート

### Q1-1: 同じ `docker container run` コマンドを2回実行すると、1回目と2回目で違いはありますか？どう違いますか？

【回答欄】
違いが無い
### Q1-2: なぜ違いますか？

【回答欄】
１回目にdocker container run ubuntu:latest /bin/echo 'Hello world'　全部入れて実行したから
### Q1-3: `docker container ls` と `docker container ls -a` はどう違いますか？

【回答欄】
一つ目の方は起動中のものが表されて、二つ目の方は過去に起動したものも表される
### Q1-4: `docker image ls` と `docker container ls -a` はどう違いますか？（間違ってもいいので、自分の考えを述べてください）

【回答欄】
imageのほうではSIZEも現れているが、containerの方はSIZEは出ていない
### Q1-5: `ubuntu` イメージでの `cat /etc/issue` の結果をペーストしてください

【回答欄】
Ubuntu 18.04.3 LTS \n \l
### Q1-6: `docker image ls` と `docker container ls -a` はどう変化しましたか？

【回答欄】
imageのほうでは変化ないがcontainerの方では、一つコンテナが増えている。
### Q2-1: `-d` (デタッチド・モード) でコンテナを起動すると、どのような状態になりましたか？

【回答欄】
なにも変化を感じない
### Q2-2: http://localhost/ をブラウザで開くと、何が表示されましたか？

【回答欄】
Welcome to nginx!
### Q2-3: コンテナの起動時と終了時で、docker container ls -a はどのように変化しましたか？

　[回答欄]
nginxの部分が、起動時ではup ◯　minutesと表示されていたが終了時ではExitedと表示されていた。
### Q3-1: `docker build -t sample-image .` 実行時に表示されている `building...` は、Dockerfileのどの行から実行されましたか？

【回答欄】
上の行から
### Q3-2: `docker run sample-image` を実行すると、どうなりましたか？

【回答欄】
Switch to inspect mode.と表示された