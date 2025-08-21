# Perspect

### 📖 概要

「**Perspect**」は、複数の生成AIがディベート形式で議論を行い、その結果をユーザーに提供するWebサービスです。このサービスは、明確な答えのない複雑な議題に対し、多角的な視点を提供し、ユーザーの意思決定を補助することを目的としています。司会進行AI、肯定側AI、否定側AIの3つの役割をAIに与え、論理的で分かりやすい議論を自動生成します。

### ✨ 主な機能

  * **AIディベート**: テーマを入力すると、3体のAIがリアルタイムでディベートを開始します。
  * **議論の要約**: ディベート終了後、議論の主要な論点をまとめた要約が自動で生成されます。
  * **PDFダウンロード**: 議論の全ログと要約をPDF形式でダウンロードできます。ユーザーのプライバシー保護のため、サーバーに議論履歴は保存されません。

### 🛠 技術スタック

このプロジェクトは、モダンなWebアプリケーション開発のベストプラクティスを取り入れた構成で開発されています。

  * **フロントエンド**:
      * **Next.js 15**: Reactベースのフルスタックフレームワーク
      * **React 19**: UIコンポーネントライブラリ
      * **TypeScript**: 型安全なJavaScript
      * **TailwindCSS**: ユーティリティファーストのCSSフレームワーク
      * **Shadcn UI**: 再利用可能なUIコンポーネントライブラリ
      * **React Hook Form**: フォーム管理ライブラリ
  * **バックエンド**:
      * **Next.js API Routes**: サーバーレス関数としてAPIを構築
  * **データベース**:
      * **Supabase**: 認証機能
      * **Prisma**: ORM (Object-Relational Mapper)
      * **PostgreSQL**: データベース
  * **デプロイ**:
      * **Vercel**: ホスティングプラットフォーム
  * **AI API**:
      * **OpenAI API**: AIモデル（GPT-3.5-Turbo, GPT-4o）の利用

### 🚀 開発環境のセットアップ

#### 1\. リポジトリをクローン

```bash
git clone [リポジトリのURL]
cd perspect
```

#### 2\. 依存関係のインストール

```bash
npm install
# または
yarn install
```

#### 3\. 環境変数の設定

プロジェクトルートに`.env.local`ファイルを作成し、以下の情報を設定します。

```env
# Supabase
NEXT_PUBLIC_SUPABASE_URL=YOUR_SUPABASE_URL
NEXT_PUBLIC_SUPABASE_ANON_KEY=YOUR_SUPABASE_ANON_KEY

# OpenAI API
OPENAI_API_KEY=YOUR_OPENAI_API_KEY
```

#### 4\. ローカル開発サーバーの起動

```bash
npm run dev
```

### 🤝 貢献

バグ報告や機能提案、プルリクエストを歓迎します。貢献についての詳細は、`CONTRIBUTING.md`ファイルをご覧ください。

### 📄 ライセンス

このプロジェクトは[ライセンスの種類]のもとで公開されています。

```
```