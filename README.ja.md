# music-brainstorming-bgm

ブレインストーミング中の集中力と創造力を高めるために設計された、AI生成によるインストゥルメンタル楽曲のコレクションです。本リポジトリでは、楽曲の視聴や生成に使用されたプロンプトを閲覧できるWebベースの音楽プレイヤーを提供しています。

## デモ

[**▶️ ブラウザで聴く**](https://code4fukui.github.io/music-brainstorming-bgm/)

プレイヤーは、プレイリスト、再生中の楽曲のアルバムアートとオーディオコントロール、AI生成プロンプトを表示する3ペイン構成のインターフェースを備えています。

## 機能

- **Webベースのプレイヤー**: 最新のブラウザで動作する、シンプルな静的HTMLプレイヤーです。
- **AIプロンプトの表示**: Suno AIで各楽曲を生成する際に使用されたプロンプトをそのまま表示します。
- **ネイティブメディアコントロール**: Media Session APIを利用し、OSのメディアコントロール（ロック画面やキーボードショートカットなど）と連携します。
- **オープンデータ**: すべての楽曲、画像、メタデータは本リポジトリに含まれており、再利用が可能です。

## データソース

楽曲は[Suno](https://suno.com/)を使用して生成されました。

- **オリジナルのSunoプレイリスト:** [https://suno.com/playlist/ed50f5df-5017-4e51-b88a-9aadf3ca025d](https://suno.com/playlist/ed50f5df-5017-4e51-b88a-9aadf3ca025d)

プレイリストのデータと音声ファイルは、[music-opendata-fukui](https://github.com/code4fukui/music-opendata-fukui)プロジェクトのスクリプトを使用してダウンロードおよびローカライズされています。以下のDenoコマンドを実行することで、このプロセスを再現できます。

```sh
deno run -A https://code4fukui.github.io/music-opendata-fukui/download.js ed50f5df-5017-4e51-b88a-9aadf3ca025d
```

## 使い方

プレイヤーをローカルで実行するには、本リポジトリをクローンし、Webブラウザで`index.html`ファイルを開いてください。

```bash
git clone https://github.com/code4fukui/music-brainstorming-bgm.git
cd music-brainstorming-bgm
# ブラウザでindex.htmlを開く
```

## ライセンス

本リポジトリのコンテンツは、CC0ライセンス（パブリックドメイン）の下で提供されています。
