## 各種情報
**サービスの概要とMVPで検証する事柄：**  
VegeGuideは、健康を意識し始めた忙しい社会人男性に向けて、旬の野菜情報・地域別価格比較・レシピ提案・買い物リスト・食材管理を一元化するWebアプリです。  
MVPでは、「旬・安価・栄養価の高い野菜」を起点に、時短レシピを提案し、買い物リストまでを自動で生成する導線を提供することで、ユーザーが継続的に活用したくなるかを検証します。

**サービス名：**  
VegeGuide（ベジガイド）

**サービスURL：**  
https://vegeguidefrontend.vercel.app/

---

## READMEレビュー時にMVPリリース時点で実装予定だった機能
- [ ] ユーザー登録機能（JWT + Cookieベース）
- [ ] ログイン・ログアウト機能
- [ ] 野菜一覧表示（旬・価格・栄養価で並び替え可能）
- [ ] 野菜詳細表示（基本情報＋レシピ生成）
- [ ] レシピ表示機能（レシピ一覧・詳細）
- [ ] 買い物リスト自動生成機能（レシピから）
- [ ] 買い物リストのチェック機能
- [ ] デプロイ（Vercel, Render）
- [ ] Sidekiqによる価格情報の定期更新

---

## READMEレビュー時から変更した機能
- **価格情報の定期更新（Sidekiq）**：サーバー運用コストの観点から保留。本リリースの際に実装予定。
- **価格・栄養素による並び替え**：データ量が増えてからの実装を予定。現時点では簡易表示のみ。

## サービスイメージがわかるようなスクリーンショット等

### トップページ
[![Image from Gyazo](https://i.gyazo.com/032d1cfd581d1a80715639b967a738e9.png)](https://gyazo.com/032d1cfd581d1a80715639b967a738e9)

### 野菜一覧画面
[![Image from Gyazo](https://i.gyazo.com/bbcefb674e8d2851dabf38d2eef87350.jpg)](https://gyazo.com/bbcefb674e8d2851dabf38d2eef87350)

### 野菜詳細画面
[![Image from Gyazo](https://i.gyazo.com/ba07f83b9090c03dcd98f68c3b4adf20.png)](https://gyazo.com/ba07f83b9090c03dcd98f68c3b4adf20)

### 野菜レシピ生成画面
[![Image from Gyazo](https://i.gyazo.com/5324a9b04447ab04239f817b93092dbb.png)](https://gyazo.com/5324a9b04447ab04239f817b93092dbb)

### 買い物リスト画面
[![Image from Gyazo](https://i.gyazo.com/9789b11e9cb4ee40532202dfd1a37bd9.png)](https://gyazo.com/9789b11e9cb4ee40532202dfd1a37bd9)

### 買い物リスト詳細画面
[![Image from Gyazo](https://i.gyazo.com/a7a5ab734d629cef94d0b5cc0d4826a9.png)](https://gyazo.com/a7a5ab734d629cef94d0b5cc0d4826a9)

### 登録レシピ一覧画面
[![Image from Gyazo](https://i.gyazo.com/57a9d4be0d6a3ea4d29b1bae1439e9eb.png)](https://gyazo.com/57a9d4be0d6a3ea4d29b1bae1439e9eb)

### 登録レシピ詳細画面
[![Image from Gyazo](https://i.gyazo.com/c53a3e266e9980a705b2c297072b27bf.png)](https://gyazo.com/c53a3e266e9980a705b2c297072b27bf)