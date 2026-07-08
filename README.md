# nuworks_marketing_ai — NUWORKS マーケティングAIサービス

NUWORKS株式会社の広告・マーケティングAIサービス紹介サイト。
トップ（`index.html`）が各サービスページ（`page-*.html`）を iframe で読み込むSPA風構成。

## 構成
- `index.html` — トップページ（サービス一覧・問い合わせ導線・iframe親）
- `page-benchmark-ad.html` — ベンチマーク広告
- `page-benchmark-recruit.html` — ベンチマーク採用広告
- `page-insta-ads.html` — インスタ広告 for 集客
- `page-insta-saiyou.html` — インスタ広告 for 採用
- `page-ai-ad.html` — AI広告
- `page-ai-video.html` — AI動画
- `page-towaman.html` — タワマンターゲティング広告
- `page-tokushoho.html` — 特定商取引法に基づく表示（SNSBRIDGE・AI広告）
- `slider-images/` — バナー/表示例画像（8点）

子ページの「戻る」は `window.parent.showTop()` を呼ぶため、index 経由の iframe 表示が前提。

## 由来
- 2026-07-08 受領：`LP構築依頼_ver2-3_完成版.zip`（本体一式）＋ `page-tokushoho.html`（単体受領）を統合
- 制作は別担当。中身の仕様は制作者に確認する。

## 受領時の申し送り（制作者確認事項）
- `index.html` から `page-tokushoho.html` へのリンクが未設置（フッター等に導線なし）
- 特商法ページの連絡先に「メールアドレスは確定次第更新します」の注記あり
- 問い合わせは `mailto:info@nuworks.jp` 方式（サーバー側フォームなし）

## 公開
- GitHub: `nuworks-intern/nuworks-marketing-ai`
- Netlify: `main` への push で自動デプロイ
