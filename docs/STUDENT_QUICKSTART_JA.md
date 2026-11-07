# Campus3D EnvSim Suite v0.1.5 — 学生向けクイックガイド

*対象：Windows / Blender 4.5 LTS | 所要時間はPC性能・通信状況・解析範囲で大きく変わります*

## 0. 何をするソフト？

都市・建築の3Dモデルについて、日時や気象条件を設定し、日射や熱環境を計算・可視化するソフトです。最初は小さなテストモデルで操作に慣れましょう。

## 1. 初回インストール

1. Blender 4.5 LTSをインストールします（4.5.15 LTSで実機確認）。
2. 配布ZIPを **Windowsで「すべて展開」** します。**BlenderのInstall from Diskには渡しません。**
3. Blenderをすべて終了し、展開したフォルダの `Install_EnvSim_Suite.cmd` をダブルクリック。
4. 確認画面で `INSTALL` と入力します。
5. Blenderを起動し、3Dビュー右側のNタブから **Campus3D Sim** を選択。
6. Blender終了後、`Check_EnvSim_Suite.cmd` を実行。9個すべて `OK` / `PASS` なら導入診断合格です。

## 2. テストモデルを作る

Blenderを閉じた状態で `Make_Smoke_Sample.cmd` を実行。生成された `EnvSim_SmokeTest_Synthetic.blend` を開きます。**地形24m四方・建物2棟**の練習用モデルです。

初期のCubeだけのシーンでは、赤い `Terrain not found` / `Package manifest not linked` という警告が表示されても正常です。まだモデルを読み込んでいないという意味です。

## 3. 4ステップで進む

| ステップ | 操作・確認 | ここを忘れずに |
|---|---|---|
| ① Model & GIS | 地形と建物が存在するか確認 | サンプルでは読み込み済み |
| ② Pre-Sim | 日付・気象データを取得してグラフを確認し、適用・Preflight | 晴れ／曇り、日時、場所が想定どおりか |
| ③ Simulation | **ALL Start** で実行。エラー時は表示内容に従って確認 | 計算中はBlenderを終了しない |
| ④ Post-Sim | Surface Temperature、MRT、SET*、WBGT等を選択し、時刻を変更 | 指標を選んだ後は表示ボタンを押す |

## 4. 温度分布が見えないとき

- 左下のカラーバーだけ見えるとき：**元Terrainが解析パッチを覆っている**可能性があります。`Prepare Clean Result View` を試してください。
- 3D Quantity と Export Quantity は別です。画面に表示する指標を変えるときは `3D Quantity` を選び、`Show Selected 3D Quantity` を押します。
- SET*などが夜間に低く見えるときはTime Indexを昼間にして比較してください。異常があれば教員に報告します。
- `Pre-Sim WARN` がある場合は、新しい計算前に日時・気象・場所の設定を確認してください。WARNを無視して適用しないでください。

## 5. 保存・提出

- 計算完了後は `.blend` を保存。解析結果は設定された結果フォルダやNPZファイルに保存されます。
- 授業で指示された形式（スクリーンショット、PNG、MP4、レポート等）で提出してください。
- テスト計算完了後は、Blenderを閉じて `Check_Smoke_Run.cmd` を実行すると構造診断ができます。

## ご注意

Campus3D Tools（3DTools）は別アドオンです。Suiteを入れても3DTools・QGIS側は変更されません。インストール済みのものを勝手に削除しないでください。

このソフトはBETA版です。計算が完了しても結果の妥当性を確認する必要があります。
