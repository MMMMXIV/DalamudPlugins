# MMMMXIV Dalamud Plugins

MMMMXIVのDalamudプラグインをまとめて配布する共通リポジトリです。

## 導入

`/xlsettings` → 実験的機能 → カスタムプラグインリポジトリに次のURLを追加し、有効化・保存してください。

```text
https://raw.githubusercontent.com/MMMMXIV/DalamudPlugins/main/repo.json
```

`/xlplugins` から必要なプラグインを選んでインストールします。今後ここに追加するプラグインも、同じURLから導入できます。

旧DSRMeteorPilotの配布URLを登録済みの場合は、旧URLを削除し、上記URLに差し替えてください。両方を登録する必要はありません。

## 配布中

| プラグイン | バージョン | ソース・説明 |
| --- | --- | --- |
| DSR Meteor Pilot (Validation) | 0.2.6.0 | [DSRMeteorPilot](https://github.com/MMMMXIV/DSRMeteorPilot) |

DSR Meteor Pilotは検証版です。移動にはvnavmeshが別途必要です。詳しい制限とビルド手順は各プラグインのソースリポジトリを参照してください。

## 配布の管理

`repo.json` はプラグイン情報の配列です。新しいプラグインを追加するときは、その情報を配列に追加します。各プラグインのソースと配布ZIPはそれぞれのリポジトリで管理できます。

更新時はDLL・マニフェスト・一覧のバージョンを揃え、ZIPの公開を確認してから一覧のダウンロードURLを更新してください。各InternalNameは一意で、公開後は変更しません。
