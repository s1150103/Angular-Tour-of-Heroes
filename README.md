# Angular Tour of Heroes - ステップ6：HTTP通信によるデータ取得

このブランチ（`tutorial/06-Get_data_from_a_server`）は、Angularチュートリアルの第6章「サーバーからデータを取得する（Get Data from a Server）」の内容を実装したものです。

## このステップで学べること

- Angularの `HttpClientModule` を使ってHTTP通信を実装
- モックサーバー（`in-memory-web-api`）からデータを取得
- `HeroService` によるデータ取得をHTTP経由に変更
- 各コンポーネントで非同期データ（Observable）を使った表示処理
- エラーハンドリングとログ出力（`MessageService`）

##  主な変更点

| ファイル | 説明 |
|--------|------|
| `app.module.ts` | `HttpClientModule` をインポート、モックAPIモジュール設定を追加 |
| `in-memory-data.service.ts` | モックのヒーローデータを提供する仮想API |
| `hero.service.ts` | `HttpClient` を用いてデータ取得を行うように変更 |
| `heroes.component.ts` | サービスを通じてヒーロー一覧を非同期で取得 |
| `hero-detail.component.ts` | IDでヒーローを取得するロジックを `HttpClient` に対応 |

##  セットアップと起動方法

```bash
npm install
ng serve

