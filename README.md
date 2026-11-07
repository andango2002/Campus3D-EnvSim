# Campus3D EnvSim Suite

**v0.1.5 BETA — Windows / Blender 4.5 LTS**

Campus3D EnvSim Suiteは、3D都市・建築モデルを用いた熱環境の学習・検討を支援するBlenderアドオン群です。モデル確認から、解析前準備（Pre-Sim）、一括計算（Simulation / ALL Start）、解析結果の表示・書き出し（Post-Sim）までを **Campus3D Sim** タブから操作します。

> **BETA / 教育・研究向け試験版。** サンプルによる実行確認はできていますが、任意のモデル・GPU・気象条件での正確性や計算成功を保証するものではありません。

## ダウンロード

GitHubの **Releases → v0.1.5-beta → Assets** から、`Campus3D_EnvSim_Suite_v0.1.5_AutoNTabs_BETA.zip` を入手してください。**Code → Download ZIP はインストーラではありません。**

## 最短インストール（Windows）

1. Blender **4.5 LTS** をインストール（実機確認は4.5.15 LTS）。
2. Suite ZIPをWindowsで右クリック → **「すべて展開」**。**Blenderの「Install from Disk」にSuite ZIPを直接読み込ませない**でください。
3. Blenderの全ウィンドウを終了。展開フォルダの `Install_EnvSim_Suite.cmd` をダブルクリックし、確認後に `INSTALL` と入力。
4. Blenderを起動。Nタブの **Campus3D Sim**（通常操作）と **EnvSim Advanced**（詳細操作）を確認。
5. Blenderを終了して `Check_EnvSim_Suite.cmd` を実行し、`9/9 PASS` を確認。

既存のv0.1.3/v0.1.4環境では `Upgrade_Workflow_Only.cmd` を使い、Workflowのみ更新できます。計算エンジンを再インストールする必要はありません。

## 初めて操作する場合

- 初期Cubeだけのシーンでは、モデル・Terrain・GISがない旨の警告が出ても**正常な未設定状態**です（v0.1.5の制約）。まだ計算しないでください。
- 小規模試験：Blenderを閉じて `Make_Smoke_Sample.cmd` → 作成された `.blend` を開く → **Campus3D Sim** の Student を選択 → Pre-Simで日時・気象を確認 → 検証後 `ALL Start` → Post-Simの結果を見る。
- 本来のGISモデルは別の作成・取込工程で用意し、解析に必要な地形・建物・材料・気象等を設定してください。Workflowの `Model & GIS` は基本的に読み取り用です。

使い方は [学生向けクイックガイド](docs/STUDENT_QUICKSTART_JA.md) を参照してください。

## 含まれるアドオン

| コンポーネント | Version |
|---|---:|
| EnvSim | 0.9.15 |
| GroundPrep | 0.3.2 |
| TreePrep | 0.3.0 |
| MeteoPrep | 0.2.0 |
| ModelPrep | 0.3.3 |
| Pre-Sim | 0.2.1 |
| Simulation | 0.1.1 |
| Post-Sim | 0.3.8 |
| Workflow | 0.3.9 |

**重要：Campus3D Tools（3DTools）およびQGISプラグイン GSI2Campus3D は同梱・変更しません。** 別プロジェクトとして管理します。

## 実機検証・既知の注意点

- Windows / Blender 4.5.15 LTSで、別PCへの一括導入、9/9 Doctor PASS、24m四方の小規模サンプルによるALL Run完了、5種類の結果ファイル検出、Nタブ自動整理を確認。
- `Pre-Sim WARN` の履歴が残ることがあります。**Simulation COMPLETE と、次の実行前に条件を再確認すべきことは両立します。** 日時・位置・気象・解析条件を確認してください。
- 初期の空シーンで赤い警告が表示されます。初回起動ガイドへの変更は次版の課題です。
- 表示が灰色なら、元のTerrainが解析パッチを覆っている可能性があります。`Prepare Clean Result View` / 表示復元機能を確認してください。
- Intel Iris XeでVulkan警告が出る場合があります。ドライバ・Blender版を確認してください。描画と計算の適合性は別途検証が必要です。
- 特定の古いBlender 4.5.x環境では気象取得でSSL証明書エラーが発生しました。4.5.15 LTSでの再試行を推奨します。SSL検証を無効化しないでください。

## リリース状態と資料

- [リリースノート](RELEASE_NOTES_v0.1.5.md)
- [学生向けクイックガイド](docs/STUDENT_QUICKSTART_JA.md)
- [教員向け授業導入メモ](docs/INSTRUCTOR_CHECKLIST_JA.md)
- [SHA-256](SHA256SUMS.txt)

公開前に、ソースコードと同梱データの利用許諾・第三者データの取り扱いを確認してください。現時点では新たなOSSライセンスを自動付与していません。
