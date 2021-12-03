# ３．事前準備

## ✅ Supabase にサインアップ

Github アカウントを使って、Supabase にログインしましょう。

### ① [Supabase](https://supabase.com/)にアクセスする。

### ② [ Start your project ] をクリックする

![gras](010_supabase-1.png)

### ③ [ Continue with GitHub ] をクリックする

![gras](020_supabase-2.png)

### ④ Github のアカウント情報を入力後、[ Sign in ] を入力してください。

![gras](030_supabase-3.png)

### ⑤ 以下のような画面が表示されれば成功です。

![gras](040_supabase-4.png)

## ✅ Gitpod にサインアップ

開発環境の構築をしましょう。

### ① [ここをクリックして Gitpod を起動](https://gitpod.io/#https://github.com/AkiUnleash/hands-on-nextjs-supabase/tree/main)

### ② 以下のような画面が表示されれば成功です。

![gras](050_gitpod-1.png)

## 🤔 RDB と NoSQL の違い

プロジェクト作成の待ち時間に、RDB と NoSQL の違いに簡単に説明します。

### NoSQL

Firebase Store には以下の３つの概念があります。

- コレクション
- ドキュメント
- フィールド

コレクション（フォルダ）の中に、ドキュメント（紙）が有り、その中にフィールド（データ）が記載しているイメージです。

### メリット

#### 高速な処理

他のプロセスと同期を取らずに、読み書きに徹しているためとにかく高速です。
