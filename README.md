# Docker Simple CI/CD Demo

## 概要

Dockerを使用したシンプルなCI/CDパイプラインのデモプロジェクトです。Udemyの「理解して使う!Docker入門＋応用」講座を通じて、コンテナ技術とCI/CDの基礎を学習しています。

## 目的

- Dockerの基本操作とコンテナ管理の理解
- Docker Composeを使った複数コンテナの管理
- CI/CDパイプラインの構築と自動デプロイの実践
- 実務で使えるコンテナ技術の習得

## プロジェクト構成

```
docker-simple-cicd-demo/
├── api/              # バックエンドAPI
├── web/              # フロントエンド
├── .github/          # GitHub Actions設定
├── .aws/             # AWS設定
└── docker-compose.yml
```

## 使用技術

- **Container**: Docker, Docker Compose
- **CI/CD**: GitHub Actions
- **Cloud**: AWS (予定)
- **Backend**: Node.js / Python (API)
- **Frontend**: React / HTML/CSS (Web)

## 学習内容

このプロジェクトを通じて以下を学習しています:

### Docker基礎
- Dockerコンテナのライフサイクル管理
- Dockerfileを使ったカスタムイメージの作成
- データ永続化の方法
- ネットワーク設定

### Docker Compose
- 複数コンテナの一括管理
- サービス間の連携設定
- 開発環境の構築

### CI/CD
- GitHub Actionsを使った自動テスト
- 自動ビルドとデプロイ
- コンテナイメージのレジストリ管理

## セットアップ

```bash
# コンテナの起動
docker-compose up -d

# コンテナの停止
docker-compose down

# ログの確認
docker-compose logs -f
```

## CI/CDパイプライン

GitHub Actionsを使用して、以下の自動化を実現しています:

1. コードのプッシュ時に自動テスト実行
2. Dockerイメージの自動ビルド
3. コンテナレジストリへのプッシュ
4. デプロイ環境への自動デプロイ

---

**開発者**: Kohei Nishiwaki  
**学習元**: Udemy - 理解して使う!Docker入門＋応用  
**更新日**: 2025年8月
