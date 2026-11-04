# Personal Obsidian Sync — GitHub Pages

Google Drive / GSync for iPhone の個人用 OAuth 連携説明サイトです。

- Homepage: https://keigo0210.github.io/
- Privacy policy: https://keigo0210.github.io/privacy.html
- OAuth callback: https://keigo0210.github.io/callback.html

## GitHub Pages 公開

1. このリポジトリの **Settings → Pages** を開く。
2. **Build and deployment → Source: Deploy from a branch** を選ぶ。
3. **Branch: main / (root)** を選んで **Save** をクリック。
4. 公開後、上記の3つのURLを開き、ページが表示されることを確認する。

## Google OAuth 設定（公開後）

1. Google Auth Platform のブランディングにホームページとプライバシーポリシーを入力する。
2. Google Search Console の **URLプレフィックス** プロパティで、このサイトの所有権を確認する。必要なら Google が発行する確認HTMLをこのリポジトリのルートに追加する。
3. Google OAuth クライアントの承認済みリダイレクトURIと、iPhone版GSyncの Sign-in redirect page の **両方** を上記の callback URL に一致させる。
4. OAuthの公開要件を確認する。Google Drive全体のアクセス権限は制限付きスコープであり、GitHub Pages作成だけで審査や公開が保証されるものではない。

**秘密情報の注意**: Client Secret、アクセストークン、リフレッシュトークン、Vaultのノートをこの公開リポジトリに書かないこと。

## 出典とライセンス

`callback.html` は [GSyncのコールバックページ](https://github.com/dg0988/ObsidianGSync/blob/main/docs/callback.html) の派生版です。元コードは MIT License, Copyright (c) 2026 dg0988。ライセンスは `LICENSE-GSYNC-CALLBACK.txt` に含まれています。
