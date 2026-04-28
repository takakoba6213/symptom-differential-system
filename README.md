# 🏥 症候別鑑別サポートシステム

> 医師の問診を **PODCAST 法** で構造化し、症候別の鑑別候補をスコア順に表示する、医療関係者向けの教育・参照用 Web アプリ。

![Status](https://img.shields.io/badge/status-prototype-blue)
![License](https://img.shields.io/badge/license-All%20Rights%20Reserved-red)
![Author](https://img.shields.io/badge/by-Takahiro%20Kobayashi%2C%20M.D.%2C%20M.F.M.-1F3864)
![PODCAST](https://img.shields.io/badge/method-PODCAST-2980b9)

---

## 🚀 アプリを開く

### ▶ [**こちらをクリックして起動**](https://takakoba6213.github.io/symptom-differential-system/)

> 上記 URL は GitHub Pages の公開後に動作します。
> リポジトリ名を変更した場合は、URL の `symptom-differential-system` 部分も置き換えてください。

---

## ✨ 主な特徴

### 完成済 4 症候

| 症候 | 鑑別 DB | 特徴 |
|---|---|---|
| 🫁 **咳嗽** | 32 疾患 | レッドフラッグ 8項目／慢性咳嗽 Common 8 疾患 |
| 💫 **めまい** | 18 疾患 | AVS / HINTS / STANDING アルゴリズム |
| ❤️ **胸痛** | 18 疾患 | 致死的 6 疾患 ＋ Common ／典型的狭心痛 3 項目 |
| 💧 **浮腫** | 多疾患 | DVT / 心腎肝 / 薬剤性 / 血管性他 |

### 各症候の 4 タブ構成

- 🔍 **鑑別アルゴリズム**：PODCAST 形式チェック → Semantic Qualifier 自動生成 → 鑑別候補のスコア順表示
- 📋 **チェックリスト**：病態・問診・診察・検査・ピットフォール（進捗をブラウザに保存）
- 👁 **一目まとめ**：レッドフラッグ／Common 疾患／フローを俯瞰
- 📚 **参考文献**：主要ガイドライン・論文へのリンク

### 拡張予定（素材揃い済）
咽頭痛 ／ 腹痛 ／ 発熱 ／ 下痢 ／ 嘔吐 ／ 失神 ／ 一過性意識消失 ／ 関節痛

---

## 🎓 PODCAST 法について

時間経過を軸に病歴を網羅的に聴取するためのフレームワーク。

| 文字 | 項目 |
|:-:|---|
| **P** | Progression（経過・進行） |
| **O** | Onset（発症様式・初発／再発） |
| **D** | Duration（持続時間） |
| **C** | Consistency（持続性・性状） |
| **A** | Aggravating / Alleviating / Associated |
| **S** | Setting / Severity（背景・重症度） |
| **T** | Timing / Trigger（時間・誘因） |

**原典：**
> Kobayashi T, Ono Y. Medical history-taking by highlighting the time course: PODCAST approach. *Diagnosis (Berl).* 2023;11(1):109-111. Published 2023 Sep 8.
>
> [📖 doi:10.1515/dx-2023-0101](https://doi.org/10.1515/dx-2023-0101)

---

## 📐 設計方針

- ✅ 患者個別データを入力・保存・送信しない（教育・参照用に徹し、薬機法上の医療機器プログラム該当性を避ける構成）
- ✅ 全コンテンツを単一 HTML ファイルに統合（外部依存ゼロ・オフライン動作可能）
- ✅ ブラウザのみで動作（サーバ・データベース不要）
- ✅ 進捗保存はブラウザの sessionStorage（個人ブラウザ内のみで完結、外部送信なし）

---

## 👤 作成者

**小林 尭広 (Takahiro Kobayashi, M.D., M.F.M.)**

[GitHub: @takakoba6213](https://github.com/takakoba6213)

- 本システムの **設計・編集・コンテンツ・実装** に関する一切の著作権は作成者に帰属します。
- 各症候のチェックリスト・鑑別データベース・Semantic Qualifier 生成ロジック・レッドフラッグ整理は、作成者の **編集著作物** として保護されます。
- PODCAST 法は学術論文として公知ですが、本システムにおける症候別の編集・整理・実装は作成者独自の編集著作物です。

---

## 📜 ライセンス

**© 2026 Takahiro Kobayashi. All rights reserved.**

無断での転載・複製・改変・再配布を禁じます。

許諾する利用：医療関係者個人による閲覧・学習・診療前後の参照。

利用許諾・商用利用・パートナーシップに関するお問い合わせは作成者まで。

---

## ⚠️ 免責事項

本システムは **医療関係者向けの教育・参照用** です。

- 個別患者の **診断・治療・受診要否を判定するものではありません**
- 最終判断は利用者自身の臨床判断によります
- 本システムの利用に起因する一切の損害について、作成者は責任を負いません

---

## 🛠 ローカルで開く

`index.html` をダウンロードしてブラウザで開くだけ。サーバー不要・インターネット接続不要で動作します。
