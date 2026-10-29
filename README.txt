パナソニック ホームズ滋賀　平屋LP GitHubテスト用（2026年10月29日版）

■ 設置先
GitHubリポジトリ：adageosaka/test_pana-hiraya
想定表示URL：https://adageosaka.github.io/test_pana-hiraya/

■ アップロードするもの
このフォルダの中身を、リポジトリの直下に配置してください。
フォルダごと一段下に入れず、index.htmlと_assetsが直下になる構成です。

index.html
_assets/
.nojekyll
_config.yml
robots.txt
README.txt

ZIP自体をアップロードするのではなく、先に展開して中身を配置してください。
.nojekyllは先頭がドットの隠しファイルです。MacではCommand＋Shift＋.で表示できます。
_config.ymlにも_assetsを含める指定を入れているため、隠しファイルを見落としても
通常のGitHub Pagesで画像・CSSが除外されない構成にしています。

■ GitHub Pagesの設定
Settings → Pages → Build and deployment
Source：Deploy from a branch
Branch：main
Folder：/ (root)

反映が完了したら上記の想定表示URLで開きます。
実際のURLはGitHub Pages設定画面に表示される案内を優先してください。

■ テスト版での調整
・本番用の広告計測（GTM）を除外
・検索向けnoindexを追加
・本番専用のfavicon／manifest参照を除外
・表示アニメーションのライブラリを同梱し、外部CDNへの依存を解消
・ライブラリが読めない場合やJavaScript無効時にも本文を表示
・画像、本文、予約リンクなどは10月29日本番用と同じ内容

予約・資料請求ボタンは本番フォームへリンクします。
このフォルダはテスト用です。本番の納品データとは分けて使用してください。

■ 公式手順
https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site
