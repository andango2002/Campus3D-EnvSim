# Campus3D EnvSim Suite v0.1.5 — 授業導入チェックリスト

## 配布前

- Windows / Blender 4.5 LTS（実機確認4.5.15）を導入済みか。
- 学生がSuite ZIPを **解凍してから** `Install_EnvSim_Suite.cmd` を実行することを周知。
- Blenderを閉じてインストールし、`Check_EnvSim_Suite.cmd` で9/9 PASSを確認。
- 初期Cubeでの未リンク警告は未設定状態であり、故障ではないと説明。
- 初回は小型サンプルだけで実行。大規模GISは別日に試す。

## 授業中の流れ

1. `Make_Smoke_Sample.cmd` を実行してサンプル`.blend`を作る。
2. Workflowを `Student` に切り替え、Model & GISの地形・建物を確認。
3. Weather Explorerで日時・日射・雲量を確認し、Pre-Simのチェック結果を読む。
4. ALL Startで完了まで進める。
5. Post-SimでSurface Temperature / MRT / SET* / WBGTを切り替える。
6. 計算結果と条件を記録し、提出。

## よくあるトラブル

- **SSL certificate verify failed**：PC日時、Blenderのバージョン、OS/証明書・ネットワークを確認。SSL検証を無効化しない。
- **Vulkan警告**：特定GPUの警告は必ずしもアドオン導入失敗ではない。性能・描画は別途確認。
- **色分布が見えない**：元Terrainの重なり／ビュー表示、3D QuantityとExport Quantityの区別。
- **Pre-Sim WARN**：前回の検証履歴か現在の問題かを区別し、新しい計算前に再検証。
- **プラグインが見つからない**：SuiteをBlenderへ直接Install from Diskした可能性。ZIP展開→cmdの順序を確認。

## 今後の改善（v0.1.6で予定）

初期空シーンの赤い警告を抑え、`Campus3Dモデルを読み込んでください` と案内するWelcome状態を追加。現行v0.1.5に後付けでコード変更しないこと。
