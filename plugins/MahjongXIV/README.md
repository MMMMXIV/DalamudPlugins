# MahjongXIV 日本語対応版

FFXIV のドマ式麻雀用プラグイン [MahjongXIV](https://github.com/kuchris/MahjongXIV)（kuchris 氏作、
Xeldar Alz 氏の FFXIV-AutoMahjongSolver のフォーク）に、日本語対応と推奨表示の改良を加えた版です。

| ファイル | 内容 |
| --- | --- |
| `MahjongXIV-0.3.0.0.zip` | Dalamud が読み込む配布 ZIP |
| `MahjongXIV-0.3.0.0-src.zip` | この ZIP をビルドした完全なソースコード（AGPL-3.0） |
| `changes-from-kuchris-MahjongXIV.patch` | 元リポジトリ（コミット `ccebf3d`）からの差分 |

## 0.3.0.0 の変更点

- UI の日本語化（設定 → 表示言語：自動／English／日本語）。牌は「5萬・3筒・7索・東・白・發・中」で表示
- 日本語クライアントの自風・リーチ表示・鳴きボタン（ロン／ツモ／リーチ／ポン／九種九牌／パス など）を認識
- 推奨表示を自動打牌と同じ判断に統一（見えている牌・ドラ・他家リーチ時のベタオリ・フリテン回避・リーチ判断）
- 有効牌・リーチ者・ロン可能・リーチ中のツモ切りを表示。待ち時間を初期値に戻すボタンを追加

使い方は `/mj` でウィンドウを開き、「推奨表示」か「自動打牌」を選んで「開始」を押します。詳しくはソース内の
`README.ja.md` を参照してください。

## 注意

- 元の MahjongXIV と同じ InternalName（`MahjongXIV`）です。kuchris 氏のリポジトリも登録している場合は、
  どちらか一方だけを有効にしてください。
- 日本語クライアントのゲーム内文字列はまだ実機検証が十分ではありません。誤認識があれば `/mj state` と
  `/mj options` の `/xllog` 出力を添えて報告してください。
- 他のプレイヤーと対戦するミニゲームの自動化は FFXIV の利用規約に反します。自動打牌は自己責任で使用してください。

ライセンス: GNU AGPL v3.0 以降（ソース ZIP 内の `LICENSE.md` と `NOTICE` を参照）。
