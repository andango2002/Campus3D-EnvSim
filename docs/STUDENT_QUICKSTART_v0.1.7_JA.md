# Campus3D EnvSim v0.1.7 BETA — 学生向け簡易ガイド

1. 教員の案内に従ってQGIS／Campus3D Toolsで対象街区を読み込み、地理空間モデルを作成する。
2. EnvSim Suiteを導入済みのBlender 4.5を起動し、Nパネルの `Campus3D Sim` → `Student` を確認する。
3. 日付をカレンダーから選び、**Fetch / Preview Selected Day** でその日の気象条件を確認する。
4. **Use This Day + ALL Start** で計算を開始する。前日24時間の助走を内部で実施後、対象日の結果を計算する。
5. Post-Simでは、時間を変えてSurface Temperature / MRT / SET* / WBGTを観察する。3D凡例にJST日時と外気温Taが表示される。
6. 夜間や日陰／日向の違い、屋根・道路の違いを考察する。解析値はモデルの仮定に依存し、実測値と一致すると保証されるものではない。

気象取得に失敗したらそのまま実行せず、教員に相談してください。大規模モデルで容量エラーが出たら、QGIS側で領域や解像度を見直してください。
