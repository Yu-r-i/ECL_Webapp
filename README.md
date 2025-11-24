# ECL Web Archive System  
研究室内のレポート・卒業研究を階層管理し、ブラウザから閲覧できるアーカイブ管理システム

---

## Overview  
本プロジェクトは、研究室内に蓄積された PDF / Markdown / テキスト資料を  
ディレクトリ構造を保持したまま Web 上で検索・閲覧できるアーカイブ管理システムです。

従来は NAS に散在していた資料を整理し、  
年度 → 学籍番号 → サブディレクトリ → ファイル という構造でブラウザに表示します。  
PDF プレビューやテキストのハイライト表示にも対応しています。

研究室内サーバー（オンプレ環境）で動作する前提で設計されています。

---

## Features  
- 年度・学生ごとのディレクトリ構造をそのまま表示（Finder風 UI）  
- PDF・画像・テキストファイルのブラウザ上でのプレビュー  
- MongoDB による柔軟なメタデータ管理  
- Express API によるファイル情報の提供  
- React によるインタラクティブなフロントエンド  
- Docker（nginx / node / mongo）による統合動作環境  
- Python スクリプトで数万件のファイル情報を自動登録

---

## Technologies  

### Frontend
- HTML
- CSS
- React

### Backend
- JavaScript
- Node.js / Express  
- MongoDB  

### Infrastructure
- Docker（nginx / node / mongo）  
- Python（メタ情報抽出スクリプト）

---

## Setup (Docker)

### 1. Build & Run
~~~bash
docker-compose up --build -d
~~~

### 2. Access
- Web App: http://localhost:8080/seminar/
- API Endpoint: http://localhost:8080/api/files
- MongoDB: mongodb://localhost:27017

---

## Author

近畿大学 情報学部 情報学科
サイバーセキュリティコース
電子商取引研究室（ECL）
舩戸 雄吏（Funato Yuri）
