
[English](README.md) | 日本語 | [한국어](README.kr.md)

  

# easy-notion-blog

  

[![GitHub stars](https://img.shields.io/github/stars/otoyo/easy-notion-blog)](https://github.com/otoyo/easy-notion-blog/stargazers)

[![GitHub license](https://img.shields.io/github/license/otoyo/easy-notion-blog)](https://github.com/otoyo/easy-notion-blog/blob/master/LICENSE)

  

<img src="https://user-images.githubusercontent.com/1063435/201917958-432ebbcb-6960-4106-8fd2-9ddcd7539781.jpg" width="480">

  

あっという間に Notion Blog を始めることができていた...
easy-notion-blogの **【魔改造版】**

==作りやすさ==を重視しているため、
必要最小限のコードに留めています。

- :rocket: Next.js最新版に対応しているためページの読み込みが**爆速**

- :pencil: **自分の~~Notion~~ Obsidianで**ブログが書ける

- :hammer_and_wrench: ブログの見た目を**自分好みにカスタマイズ可能**

- :white_check_mark: **~~Notion 公式API~~ Obsidian プラグイン**を使っているので~~安心~~ 簡単なコードで実現


オリジナルで改造するために参考になるeasy-notion-blogのコードを残しています。
改造する上で参考になる記述が沢山あるので、のぞいてみてください⭐

[easy愛好家が集まってこっそり開発継続中のeasy-notion-blog](https://github.com/herohoro/zutto2_easy-notion-blog)
※ 元々開発されていたotoyoさんは[astro-notion-blog](https://github.com/otoyo/astro-notion-blog)の開発に専念しています  



## スクリーンショット

  

### :camera_flash: ブログ側

  

<img src="https://user-images.githubusercontent.com/1063435/201293737-63c0d504-d34b-4500-98ab-808f4d2e89f3.png" width="600">

  

### :camera_flash: Notion側

  

<img src="https://user-images.githubusercontent.com/1063435/201301619-54cf07da-e638-4751-b56c-7115ed5d4eb0.png" width="600">

  

## クイックスタート

  

### 必要要件

  

- [Vercel](https://vercel.com/) アカウント

- Git

  

### 手順

  


6. [vercel.com](https://vercel.com/) にログインします

7. プロジェクトを新規作成しリポジトリとして `otoyo/easy-notion-blog` をインポートします(チームの作成はスキップします)

8. "Configure Project" で "Environment Variables" を開き先ほどメモした `NOTION_API_SECRET` と `DATABASE_ID` を入力します

9. デプロイが完了すると Notion Blog が見えるようになります

  



  

## デモ

  

[https://easy-notion-blog-otoyo.vercel.app/blog](https://easy-notion-blog-otoyo.vercel.app/blog)

ユーザーブログは [wiki](https://github.com/otoyo/easy-notion-blog/wiki/Users%27-blogs-%E3%83%A6%E3%83%BC%E3%82%B6%E3%83%BC%E3%83%96%E3%83%AD%E3%82%B0) から見ることができます。

  

## カスタマイズするには

  

### 追加の必要要件

  

- Node.js v16 もしくはそれ以上

- [Yarn](https://yarnpkg.com/getting-started)

- [direnv](https://github.com/direnv/direnv)

  

### 手順

  

1. このリポジトリをフォークしてローカルに clone します

2. プロジェクトルートで direnv を使って下記の環境変数を設定します

  

```sh

direnv edit .

```

  

```sh

export NOTION_API_SECRET=<YOUR_NOTION_API_SECRET>

export DATABASE_ID=<YOUR_DATABASE_ID>

```

  

3. 依存関係をインストールしローカルサーバーを起動します

  

```sh

# 依存関係のインストール

yarn install

  

# 開発サーバー(localhost:3000) の起動

yarn dev

```

  

4. ブラウザで [http://localhost:3000](http://localhost:3000) を開きます

  

開発環境では `Published` でないエントリーも表示されるためプレビューすることができます。ただし `Slug` が設定されていないエントリーは表示されません。

  

5. 開発サーバーを停止するにはターミナルで `Ctrl+C` を押します。

  

### その他の情報

  

[wiki](https://github.com/otoyo/easy-notion-blog/wiki) をご覧ください。

  

## バグ報告 & 機能要望

  

Issue を作成してください。日本語で大丈夫です。

  

## :bird: Twitter コミュニティ

  

最新のアップデート情報を受け取ったり、カスタマイズに困った際に他のメンバーのサポートを得ることができます。

  

- [easy-notion-blog](https://twitter.com/i/communities/1497431576975908868)

  

## 貢献

  

PR 歓迎です。

  

---

  

easy-notion-blog は [ijjk/notion-blog](https://github.com/ijjk/notion-blog) と [otoyo/notion-blog](https://github.com/otoyo/notion-blog) をベースにしています。