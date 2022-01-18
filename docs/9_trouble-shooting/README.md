# トラブルシューティング

## ４．プロジェクトの作成

### yarn build 時にエラーが発生する。

以下のようなエラーコードが出力されてビルドできない。

```
Error: Missing env.NEXT_PUBLIC_SUPABASE_URL
    at Object.8786 (/workspace/hands-on-nextjs-supabase/.next/server/chunks/610.js:80:9)
    at __webpack_require__ (/workspace/hands-on-nextjs-supabase/.next/server/webpack-runtime.js:25:42)
    at Object.7448 (/workspace/hands-on-nextjs-supabase/.next/server/pages/_app.js:35:19)
    at __webpack_require__ (/workspace/hands-on-nextjs-supabase/.next/server/webpack-runtime.js:25:42)
    at __webpack_exec__ (/workspace/hands-on-nextjs-supabase/.next/server/pages/_app.js:235:39)
    at /workspace/hands-on-nextjs-supabase/.next/server/pages/_app.js:236:66
    at Function.__webpack_require__.X (/workspace/hands-on-nextjs-supabase/.next/server/webpack-runtime.js:108:21)
    at /workspace/hands-on-nextjs-supabase/.next/server/pages/_app.js:236:47
    at Object.<anonymous> (/workspace/hands-on-nextjs-supabase/.next/server/pages/_app.js:239:3)
    at Module._compile (node:internal/modules/cjs/loader:1101:14) {
  type: 'Error'
}
error Command failed with exit code 1.
```

#### 原因と対策

.env.local に API キーが保存されていない可能性があります。
「✅ API キーを保存」を参照しながら、.env.local に API キーを保存してみてください。

## Github ログインの構築

### 設定して試したけど、ログインができない。

#### 考えられる原因

- 『② 必要な３つの情報を入力 → Register application をクリック。』の”Authorization callback URL”の設定値、Supabase の URL と”/auth/v1/callback”が入力されているか確認してください。
- Supabase に値を設定した後に、必ず Save が必要です。上部に Save ボタンがあるので、押下したあとに再度ログインをためしてみてください。
