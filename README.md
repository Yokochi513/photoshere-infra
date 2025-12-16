# photoshere-infra

「ひかりの跡（灯の跡）」プロジェクトの  
**インフラ・開発環境を統合管理するリポジトリ**です。

本リポジトリは以下を目的としています。

- フロントエンド / バックエンドの一括起動
- マシン差異のない開発環境構築
- Docker / docker-compose による環境統一
- 将来の CI / 本番環境への拡張

---

## リポジトリ構成

```text
photoshere-infra/
├─ docker-compose.yml          # 開発用
├─ docker-compose.prod.yml     # 本番用（将来）
├─ .env.example
├─ .gitignore
├─ README.md
│
├─ backend/    # backend リポジトリ（Git submodule）
├─ frontend/   # frontend リポジトリ（Git submodule）
└─ mongo/
