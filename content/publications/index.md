---
title: Publications
date: 2022-07-29 09:00:00
---
# Publication
This is home for my research publications, each linked with accompanying preprints.
## 2022
### A study on daylight patterns and the related impacts on subjective glare perception
* Manuscript currently in preparation, soon to be submitted

### A comparison study on different HDR-imaging technologies for glare studies
* Manuscript currently in preparation, soon to be submitted

### A  wearable high dynamic range imager for glare studies: calibration and application
* Manuscript currently in preparation, soon to be submitted

## 2021
### [Creatinng positive atmosphere and emotion in an office-like environment: A methodology for the lit environment](https://discovery.ucl.ac.uk/id/eprint/10127368/1/KIM_MANSFIELD_2021.pdf)
* In this study, participant emotion states were investigated when experiencing fifteen different lighting schenarios (concept design were  provided by professional lighting designer). The results indicated that positive emotions of *liveliness* could be cued under two lighting settings and that of *relaxation* under three lighting settinngs (of varying colour temperatures and light distribution). This study used bivariate 2-d kernel density estimates to differentiate emotions between 15 different lighting conditions on an *unpleasantness-pleasantness* and *activation-sleepiness* grid.
* Authors: **Dong Hyun Kim** and Kevin Mansfield
* *Building and Environnment* May 2021

## 2020
### [Clustering of office workers from the OFFICAIR study in The Netherlands based on their self-reported health and comfort](https://www.sciencedirect.com/science/article/pii/S0360132320302195)
* [OFFCIAR](https://cordis.europa.eu/project/id/265267/reporting) was a European collaborative project, with an intentiion of a better understanding of factors affecting the indoor environment in modern office buildings. This study analysed the data from the Netherlands. The results indicated that females workers and the workers in open-plan offices reported signficianly more symptoms and compaints. TwoStep cluster analysis revealed three different profiles of office occupants based on their health symptoms and IEQ-related needs. Detailed descriptions of these three profiles were provided in this paper. This paper suggests that there is a need of an integrated approach to provide customized solutions for the differennt office workers who differed in their health problems and IEQ needs
* Authors:  **Dong Hyun Kim**, Philomena Bluyssen
* *Building and Environnment* June 2020

### [First results of self-reported health and comfort of staff in outpatient areas of hospitals in the Netherlands](https://www.sciencedirect.com/science/article/pii/S0360132320302304)
* To be added
* Authors: AnneMarie Eijkelenboom*, **Dong Hyun Kim**, Philomena Bluyssen
* *Building and Environnment* July 2020


## アクティビティ

### レイアウトダイアグラム

* シーエンス：　より高度で複雑な自動化に向こう
* フローチャート：　シンプルな自動化プロジェクトに適している
* ステートマシン
* Global Exception Handler (グローバル例外ハンドラー)

>参照：[https://docs.uipath.com/studio/lang-ja/docs/workflow-design](https://docs.uipath.com/studio/lang-ja/docs/workflow-design)

### 選択肢

* 条件分岐(If)：　シーケンス用条件分岐
* フロー条件分岐(flow desicion)：　フローチャート用条件分岐
* フロースイッチ (Flow Switch)

### 繰り返し

* 繰り返し（前判定）(While)
* 繰り返し（後判定）(Do While)
* 繰り返し（コレクションの各要素）(For Each)

### データ操作

* CSVを読み込み(Read CSV)
    - オプションにエンコーディングを指定できる（日本語データがある場合、`"SHIFT-JIS"`を指定する）
    - 列名を含める(IncludeColumnNames)を指定できる
    - 出力タイプ：`System.Data.DataTable` [Microsoft Docs](https://docs.microsoft.com/ja-jp/dotnet/api/system.data.datatable?view=netframework-4.8)
    - `Select`メソッドで半角スペースを含む列名で指定する場合、半角スペースが特殊文字ではなく文字列として認識されるため、`[]`で列名を囲う

```
Names.Select("[メンバー ステータス] = 'Yes'")
```

### その他

* メッセージボックス
* 代入(assign)
* 待機 (Delay)
* 入力ダイアログ（input dialog）:
* フォルダーを選択(Select Folder)
* 一行を書き込み(Write Line)：　Debug用？
* アプリケーションを開く(Open Application)
* ブラウザを開く(Open Browser)
* ブラウザーにアタッチ(Attach Browser)
* 文字を入力(Type Into)
* ハイライト(Highlight)
* [アンカーベース(Anchor Base)](#アンカーベース-Anchor-Base)
* スクリーンショットをと撮る(Take Screenshot)
* 要素の有無を検出(Element Exists)
* 要素の消滅を待つ(Wait Element Vanish)

## レコーディング機能

<span style="color: green">\[○\]レコーディング可</span>
* 左クリック
    - ボタン
    - チェックボックス
    - ドロップダウン
    - ...
* 文字入力

<span style="color: red">\[×\]レコーディング不可</span>
* ショットカットキー
* 修飾キー（`ctrl + c`など）
* 右クリック
* マウスホバー

**ショットカット**
* F2 - 時間差で選択
* F3 - 領域を選択

### ベーシック

* 適する操作内容：複数ウィンドウ上の単一の操作
* 生成されるワークフローがシンプル

### デスクトップ

* 適する操作内容：同一ウィンドウ上の連続した操作
* 生成されるワークフローが複雑
* セレクターの保守性が良い

### ウェブ

ウェブアプリとブラウザーでレコーディングを行うためのものです。コンテナーを生成し、既定で 入力をシミュレート (Simulate Type)/クリック (Click) の入力メソッドを使用します。

## 入力/出力方法まとめ

### 入力

* デフォルト(Default)
    - 互換性が高い
    - キーボード対応
* ウィンドウメッセージ(Windows Message)
    - バックグラウンド処理
    - キーボード対応
* シミュレート(Simulate Type/Click)
    - 互換性が低い
    - バックグラウンド処理
    - フィールド内自動削除

### 出力

* フルテキスト(FullText)
    - スピード：★★★★★
    - 正確さ：100%
    - バックグラウンド処理
    - 非表示の項目を取得
* ネイティブ(Native)
    - スピード：★★★★
    - 正確さ：100%
    - 文字情報を取得
* OCR
    - スピード：★★
    - 正確さ：98%(?)
    - 文字情報を取得
    - CITRIX対応

## セレクター

* 部分セレクター
* 完全セレクター
* 動的なセレクター：ワイルドカードを使ってる
* アンカーベース(Anchor Base)
* 相対的なアンカー(Select Relative Element)

>セレクターがあまり安定しないと考えられるときには、[Anchor Base（アンカーベース）] アクティビティや、UiPath Explorer の [Select Relative Element（相対的なアンカーを選択してください）] を使用することで、信頼性の高い自動化を構築できる場合があります。

### アンカーベース(Anchor Base)

アンカーとして使用できるアクティビティ：
* 要素を探す(Find Element)
* 画像を探す(Find Image)

## EXCEL操作

* EXCELアプリケーションスコープ(Excel Application Scope)
* 範囲を追加(Append Range)
* データテーブルを並べ替え(Sort Data Table)
* データテーブルをフィルタリング(Filter Data Table)
* Build Data Table
* Generate Data Table
* Output Data Table

## PDF操作

PDF Activities Pack
`UiPath.PDF.Activities`

* PDFのテキストを読み込み(Read PDf Text)
    - 範囲(Range)：ページ範囲を指定する。ディフォルトは`"ALL"`。例： `1` `3-5`	
* OCRでPDFを読み込み(Read PDF With OCR)
* 画面スクレイピング(Screen Scraping)も適用

## MAIL操作

MailMessageの型：
```
System.Net.Mail.MailMessage
System.Web.Mail.MailMessage
```

* SMTP
* POP3
* IMAP
* Outlook
* Exchange
* IBM Notes

## Debug

* トライキャッチ(Try Catch)
* メッセージをログ(Log Message)
    - Critical
    - Error
    - Warning
    - Information
    - Trace
    - Verbose: Traceと同じレベルだが、アクティビティ start および end の両方のメッセージと、使用される変数および引数の値を記録する
