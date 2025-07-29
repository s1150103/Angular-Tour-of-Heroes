# Angular Tour of Heroes - ステップ5：ルーティングとナビゲーションの追加

このプロジェクトは、Angular公式チュートリアル「Tour of Heroes」におけるステップ5の内容を実装したものです。  
このステップでは、アプリケーションにルーティングと画面遷移機能を追加しました。

## ✅ このステップで行ったこと

- Angularのルーター機能を導入（AppRoutingModuleを作成）
- 以下のルートを定義：
  - `/dashboard` → `DashboardComponent`
  - `/heroes` → `HeroesComponent`
  - `/detail/:id` → `HeroDetailComponent`（パラメータ付きルート）
  - `/` → `/dashboard` にリダイレクト
- `<router-outlet>` を使用して、ルーティングビューの表示場所を指定
- 画面上部にナビゲーションリンクを追加（routerLink を使用）
- ヒーロー一覧やダッシュボードから詳細画面に遷移可能に
- URLに直接アクセス（例：`/detail/11`）しても詳細画面を表示可能
- 詳細画面に「戻る」ボタンを追加（Locationサービスを使用）

## 🔧 試すには

```bash
ng serve

