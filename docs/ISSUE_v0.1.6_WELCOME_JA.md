# v0.1.6 — Welcome表示と初回起動時の案内

## 課題

Blender初期Cubeしかない状態でCampus3D Simを開くと、赤い警告が並び初心者にとって故障に見える。

## 期待動作

- Terrain / GISパッケージがない初期シーンでは**エラーではなく未設定（Welcome）表示**にする。
- 「まずCampus3Dモデルまたはサンプルを読み込んでください」と案内。
- Model & GISの読み取り専用であること、Campus3D Toolsは別アドオンであることを明示。
- モデルがある場合は現行のPreflight警告・安全チェックを従来通り表示（警告を隠さない）。
- Student/Researcher、Nタブ自動整理、ALL Start、Post-Sim、3DToolsの独立性を変えない。

## 受け入れテスト

1. 初期Cubeのみの新規シーンではWelcome、赤いエラーの乱立なし。
2. サンプル読み込み後に4段階のステータスが正常表示。
3. 本当にGIS/パッチ/気象が不整合の場合はWARN/FAILが引き続き表示。
4. 3DToolsには一切変更がない。
5. v0.1.5の配布ZIPのSHA-256は永久に同一のまま。
