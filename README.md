メタゲノム解析は主に以下の二つ。
16SrRNAのアンプリコンシークエンスによる細菌叢解析をメタ16S解析と呼び、組成を解析する。
細菌叢の機能まで解析するのはショットガン解析。

% git add . でステージングし（% git statusで確認できる）、% git commit -m 'hoge'でコミット。% git logでその履歴を確認できる。% git push hogehoge mainでリモートに反映。
git resetでステージングをリセット
git stashでコミットせずに一時保留
(https://tatsuno-system.co.jp/2020/07/02/blog_git-command/)

TIPS集
$ grep 検索正規表現 ファイル名
パイプ(|)で処理を繋いぐ
リダイレクト(>)で標準出力をファイルに出力し、'>>'で追記。

# ショットガン解析
[Metagenome-wide association of gut microbiome features for schizophrenia](https://www.nature.com/articles/s41467-020-15457-9)から統合失調症患者の糞便サンプルについて、メタゲノムショットガンシーケンスを行って得られたデータを１例解析した。

fastpを使い、5'と3'のクオリティの低い領域のトリミングと、残存したアダプターのトリミングをする。その際に詳細に書かれたレポートが出力される。
![report_image](https://github.com/yuto1352/hiroshima2022/blob/images/report.png)

KneadDataを使い、宿主リードをフィルタリングする。
![sendsketch_image](https://github.com/yuto1352/hiroshima2022/blob/images/Screenshot.png)
大腸菌が異様に多いところが気になる。