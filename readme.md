# サービス概要

## 「VegeGuide ― 忙しいあなたの、毎日の“ちょうどいい健康習慣”」

健康を意識し始めた社会人に向けて、旬の野菜情報・価格比較・レシピ提案・買い物リスト・食材管理を一元化するWebサービスです。  
料理のハードルを下げ、食材のムダを防ぎながら、栄養価が高くコスパの良い食生活をサポートします。

---

# このサービスへの思い・作りたい理由

30代頃から気になり始めるのが健康的な食事生活です。  
現代の多忙な社会人は健康的な食生活の重要性を認識していても、外食やコンビニ食が多くなりがちです。  
それらの課題解決のために、一気貫通で野菜生活をサポートするアプリを作成したいと考えました。

---

# ユーザー層

- 忙しい社会人男性（20代後半〜30代前半）

---

# サービスの利用イメージ

1. アプリを開くと、「旬・安い・栄養価が高い」野菜が一覧で表示される  
2. 気になった野菜をタップすると、その野菜を使った時短レシピが表示される  
3. レシピを選ぶと、必要な食材が自動で買い物リストに追加される  
4. スマホを見ながら、スーパーで迷わず効率よく買い物ができる  
5. 帰宅後はレシピ通りに、短時間で簡単に調理できる  
6. 使いきれなかった食材はアプリ内の冷蔵庫機能に登録して管理  
7. 登録された食材をもとに、次回以降のレシピが提案される  
8. 食材のムダを防ぎつつ、旬の野菜を活用して栄養バランスの良い食生活を実現

---

# ユーザーの獲得について

## Qiita / Zenn / note で開発ブログを書く（SEO対策）

### 方法

- 「Rails × Reactで食材管理アプリを作った」  
- 「旬の野菜APIの取得方法とレシピ連携」

### 目的

- エンジニア層や個人開発クラスタにリーチ → 拡散・紹介されやすい

---

# サービスの差別化・推しポイント

## 1. 旬の野菜 × 地域別価格情報 × 栄養価表示の三位一体

- **差別化点：** 他のレシピアプリや買い物アプリは、「レシピ提案」「買い物メモ」「栄養価情報」が分断されている  
- **優れている点：** 「今の旬」「価格の安さ」「栄養面」の3軸から、コスパの良い食材選びができる

## 2. 複数アプリを行き来する必要がなく、毎日の食生活がシンプルに

- **差別化点：** 他サービスは「レシピだけ」「栄養管理だけ」「冷蔵庫管理だけ」  
- **優れている点：** 「野菜を選ぶ→買う→作る→残りも使う」一連の流れを一つのサービスで完結できる

## 3. 買い物リストの自動生成 × 実用的UI

- **差別化点：** 通常の買い物リストアプリは手動入力が必要  
- **優れている点：** レシピ選択で自動生成されるチェックリスト付き買い物リストで、仕事帰りでもサクッと買い物できる

## 4. 食材の無駄を減らす「冷蔵庫機能」

- **差別化点：** 生成AIによるカスタムレシピ提案、冷蔵庫内食材に基づくリコメンド  
- **優れている点：**
  - 「今あるもので何が作れる？」がすぐにわかる  
  - 食材のムダがなくなり、食費削減＋罪悪感ゼロ

## 5. 社会人男性に寄り添った世界観とメッセージ

- **差別化点：** 多くの健康・食系アプリは「家族向け」「主婦層向け」  
- **優れている点：**  
  - ターゲットを絞ることで共感を得やすい  
  - 「ちょっとだけ健康に気を遣いたい」「でも面倒なことはしたくない」層に刺さる

---

# 他サービスとの比較表

| サービス名 | 主な特徴 | 差別化ポイント（VegeGuideとの違い） |
|------------|----------|----------------------------------------|
| クックパッド | レシピ投稿・検索 | 価格比較・食材管理がない。時短・男性向けUXではない |
| Kurashiru | 動画でわかりやすいレシピ | 見栄え重視。価格比較・冷蔵庫管理には不向き |
| Paprika（海外） | 食材管理＋買い物リスト | 日本向けデータなし、日本のスーパー向けUIではない |
| 食べチョク | 野菜購入型のD2Cサービス | 価格比較・レシピ連動なし。ECサービス寄り |

---

# ✅ MVP（最小実用製品）で必要な機能一覧

## 1. ユーザー管理

- ユーザー登録 / ログイン（基本認証）  

## 2. 旬の野菜情報

- 野菜一覧の表示（名前、画像、栄養価、価格、保存方法）  
- 地域別価格情報はAPIから取得し表示

## 3. レシピ提案

- 旬の野菜に基づくレシピ提案（Gemini API使用）  
- レシピ名、食材、調理手順の簡単な表示

## 4. 買い物リストの自動生成

- レシピ選択で自動的にリスト追加  
- 食材名・調理方法表示  
- スマホで見やすいUI（チェックボックス付き）  
- 手動での食材追加・削除も可能

---

# ✅ MVP後に段階的にリリースすべき機能（優先度順）

## ★ 重要機能

1. **食材登録（冷蔵庫）機能**  
2. **冷蔵庫にある食材からのレシピ提案**  
3. **栄養価表示機能の強化**  
4. **外部認証（Google, Apple IDなど）**
5. **SNSシェア機能（集客目的）**

## 🔼 優先度：中

- レシピの保存・お気に入り機能  
- レシピ検索機能（キーワード・食材名・調理時間・カテゴリー）  
- 食材の価格履歴・比較表示（簡易グラフ）

## 🔼 優先度：低（ユーザー増加後に検討）

- 食材の賞味期限通知・自動リマインド  
- 栄養管理・目標設定（例：1日○品目）  
- LINE連携・通知機能

---

# 実装方針

---

## 1. 旬の野菜情報（地域別価格情報の取得）

- **難易度**: 中〜高  
- **難しい点**: 地域別価格情報を外部APIから取得し、表示する部分が難しい。特に、APIの取得・整形処理と価格情報の正確性を保つことが求められる。

### 実装方針:

- **API選定**  
  価格情報を取得するための信頼できるAPIを選定する。例: 公共APIや商業APIなど。

- **API通信**  
  RailsでAPI通信を行い、HTTPartyやFaradayを使用してデータを取得・整形してフロントへ渡す。

- **キャッシュ**  
  RedisやRailsのキャッシュ機能を用いて、取得データをキャッシュし、定期的に更新。

- **エラーハンドリング**  
  APIがダウンしている場合でもシステムが安定して動作するように設計する。

---

## 2. レシピ提案機能（Geminiを使用してレシピを提案）

- **難易度**: 高  
- **難しい点**: Geminiを利用したレシピ提案のロジック構築とその実装。

### 実装方針:

- **Gemini APIの導入**  
  認証やリクエスト処理など、Gemini APIの使用準備を行う。

- **レシピデータの整形**  
  食材や手順を必要な情報に絞り、見やすく表示する。

- **レシピの選択ロジック**  
  選択された野菜に基づいて、栄養素や調理法を考慮したレシピを提案するロジックを実装。

- **パフォーマンス対策**  
  処理が重くならないよう、キャッシュや非同期処理を活用する。

---

## 3. 買い物リストの自動生成

- **難易度**: 中  
- **難しい点**: 自動生成された買い物リストのUI/UX設計。

### 実装方針:

- **レシピデータの処理**  
  食材名や数量を抽出し、買い物リストへ変換。

- **UI設計**  
  Reactでチェックボックス付きの動的なリストを作成。

- **手動編集**  
  フォームでユーザーが食材を追加・削除できる機能を提供。

- **データ同期**  
  サーバー保存またはローカルストレージで状態を維持。

---

## 4. SNSシェア機能

- **難易度**: 中  
- **難しい点**: 自動でシェア文を生成し、SNSに投稿する処理。

### 実装方針:

- **SNS API連携**  
  X（旧Twitter）やInstagramのAPIを利用し、アクセストークンを取得して投稿機能を実装。

- **シェア文の自動生成**  
  「#時短レシピ #旬野菜」などのハッシュタグを自動付与。

- **UI設計**  
  プレビュー表示機能付きのシェアボタンを設置。

---

## 5. 食材の価格履歴・価格比較

- **難易度**: 中  
- **難しい点**: 店舗ごとの価格比較や履歴のグラフ表示。

### 実装方針:

- **価格履歴の保存**  
  日付ごとに価格データを保存するテーブル設計。

- **価格比較**  
  APIから複数店舗の価格データを取得し、比較可能に。

- **グラフ表示**  
  Chart.js や D3.js を用いて、Reactでグラフ表示を実装。

