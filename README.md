# AIグルコン・講座 現在地チェック

AIグルコン・講座（2ヶ月グルコン）本番までにやることを1ページのチェックリストにまとめた PWA。

- 進捗は端末内 localStorage に保存（外部送信なし）
- iOS Safari で「共有 → ホーム画面に追加」で PWA として起動
- 既存受講者向けに、これまでの複数のメール案内を1ページに集約

## 構成

- `index.html` — 本体（HTML + CSS + JS 全部インライン）
- `manifest.webmanifest` — PWA マニフェスト
- `icon-192.png` / `icon-512.png` / `icon-maskable-512.png` — アイコン

## 公開

- 公開 URL：https://mits32163216.github.io/aiglucon-checklist/
- リポジトリ：https://github.com/mits32163216/aiglucon-checklist

## 編集

`index.html` 内の `BLOCKS` 配列を編集すれば、チェック項目を追加・変更できる。localStorage キーは `aiglucon-checklist-v1`。項目 id を変更しない限り、既存ユーザーの進捗は保持される。
