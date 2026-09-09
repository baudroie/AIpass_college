# 生成AIパスポート 無料セミナー｜大学生向け

共通のReact実装から生成した大学生向けLPです。

GitHub Pages URL: https://baudroie.github.io/AIpass_college/

## 公開設定

GitHubの Settings → Pages で **Deploy from a branch**、**main**、**/docs** を選択します。
ビルド済みの公開ファイルを docs/ に含めています。GitHub Actionsでの再ビルドは不要です。

## 更新

Node.js 22以上を利用してください。

```sh
npm ci
npm run dev
npm run build
```

ソースを変更したら npm run build で docs/ を更新し、ソースと docs/ を一緒にmainへコミット・プッシュします。
共通コンポーネントは src/App.jsx、学生コピーは src/variants/student.js、社会人差分は src/variants/worker.js です。
pages.config.json がこのリポジトリの対象を指定します。画像・フォントは /AIpass_college/ 配下から読み込みます。
申込ボタンは提供済みGoogle Formsへ直接遷移します。
