社会福祉士 合格LAB v6.0｜公式過去問 自動更新版

【自動更新の仕組み】
GitHub Actions が毎週1回＋手動実行＋main更新時に、社会福祉振興・試験センターの公式「過去の試験問題」ページを確認します。

取得元:
https://www.sssc.or.jp/shakai/past_exam/index.html

- 問題文：公式の「音声読み上げ用試験問題」HTMLから取得
- 正答：公式の「合格基準・正答一覧」PDFから取得
- 問題番号が連続していることを検証
- 問題数と正答数が一致することを検証
- 各問題の選択肢が5個あることを検証
- 検証に失敗した年度は公開データへ入れない
- 新しい回が公式ページへ追加され、正答一覧まで公開されれば自動で年度一覧に追加

【重要：GitHub Pagesの設定】
このv6は GitHub Actions から直接Pagesへ公開します。
Settings > Pages > Build and deployment > Source を「GitHub Actions」に変更してください。

【リポジトリに必要なもの】
index.html
data/past_exams.js  （初期フォールバック。Actions実行時に再生成）
.github/workflows/update-past-exams.yml

【自動実行】
毎週 月曜朝ごろ（日本時間）にチェックします。
Actions画面の「Update official past exams and deploy Pages」から Run workflow を押せば、その場で手動更新もできます。

【学習履歴】
第38回の保存キーはv5と同じなので、同じ公開URL・同じブラウザなら履歴を引き継ぎます。
他年度は年度ごとに別保存です。
