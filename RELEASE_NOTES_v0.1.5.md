# Campus3D EnvSim Suite v0.1.5 BETA — Release Notes

**2026-11-07 | Pre-release | Windows / Blender 4.5 LTS**

## 主な機能

- **4段階Workflow**：Model & GIS / Pre-Sim / Simulation（ALL Start）/ Post-Sim。
- **学生／研究者UI**：Student / Simple と Researcher / Full の切替。
- **Nタブ自動整理**：Blender GUI起動後、8つの独立エンジンの設定タブを `EnvSim Advanced` に集約。普段の `Campus3D Sim` は維持。いつでも手動復元可能。
- **Weather Explorer**：日時・気象のプレビューおよび確認。気象地点と解析地点の距離検証。
- **一括計算**：日射・表面温度・MRT・SET*・WBGT等の計算フロー。
- **結果表示**：Surface Temperature / MRT / SET* / WBGT、PNG・MP4・Flight Simulationへアクセス。
- **導入診断**：Install Doctor / Project Doctor / Sample Run Verifier。

## 確認できたテスト

- 新しいWindows PCへの9アドオンの導入と `9/9 PASS`（Blender 4.5.15 LTS）。
- 小規模モデルにおける `ALL Run: COMPLETE` と、5種類のNPZ結果ファイルの検出。
- Blender GUI起動後のNタブ自動集約（Campus3D Sim / EnvSim Advanced）。
- 実機での確認は限定条件下のスモークテストであり、数値的正確性・全モデル互換を保証するものではありません。

## 既知の制約

1. 未読込の初期シーンでは赤い「Model / GIS未リンク」等の警告が表示されます。モデル読込後に検証してください。初回起動案内の改善は次版で対応予定。
2. 前回Pre-SimのWARNが履歴として残る場合があります。次の実計算前に必ず検証状態を確認してください。
3. Intel Iris Xeなど一部のGPUではVulkan初期化警告が出る場合があります。
4. 解析結果が隠れる場合は、Terrainと解析パッチの重なり・表示状態を確認してください。
5. 気象取得には接続環境・証明書ストアが必要です。SSL検証無効化による回避は推奨しません。

## 安全上の境界

**3DTools（Campus3D Tools）とQGIS側のGSI2Campus3Dは、本Suiteの配布物・更新対象に一切含まれません。** 8つの独立した計算系エンジンは元の構造を維持しています。

## インストール

1. `Campus3D_EnvSim_Suite_v0.1.5_AutoNTabs_BETA.zip` をダウンロードして展開する。
2. Blenderを閉じて `Install_EnvSim_Suite.cmd` を実行、`INSTALL` と入力。
3. Blender起動後、Nタブの自動整理を確認。
4. Blenderを閉じて `Check_EnvSim_Suite.cmd` を実行しPASSを確認。

**Suite ZIPをBlenderの「Install from Disk」に直接指定しないでください。**
