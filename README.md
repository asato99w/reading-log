# Scientific Reading Log Repository

このリポジトリは、科学書の読書記録、要約、感想を体系的にまとめるための読書記録システムです。著者別に整理され、英語・日本語の二言語対応で構築されています。

## リポジトリ構造

```
reading_log/
├── README.md              # このファイル
├── CLAUDE.md              # Claude Code用の設定ファイル
├── BIOLOGY/               # 生物学・生命科学
│   ├── Richard_Dawkins/   # 著者別整理
│   │   ├── AUTHOR.md      # 著者情報統合ファイル
│   │   ├── The_Selfish_Gene--利己的な遺伝子/
│   │   │   ├── CLAUDE.md
│   │   │   ├── README.md
│   │   │   ├── en/        # 英語版
│   │   │   │   ├── Author_Richard_Dawkins.md  # 書籍執筆時期の情報
│   │   │   │   ├── Overall_Structure.md
│   │   │   │   ├── Reading_Notes.md
│   │   │   │   └── structure/  # 章別要約
│   │   │   └── jp/        # 日本語版
│   │   │       ├── 全体構成.md
│   │   │       ├── 読書メモ.md
│   │   │       ├── 著者_リチャードドーキンス.md
│   │   │       └── 構成/  # 章別詳細
│   │   └── The_Blind_Watchmaker--盲目の時計職人/
│   ├── John_Maynard_Smith/
│   │   ├── AUTHOR.md      # 著者情報統合ファイル
│   │   └── Evolution_and_the_Theory_of_Games--進化とゲーム理論/
│   ├── Daniel_Davis/
│   │   ├── AUTHOR.md      # 著者情報統合ファイル
│   │   └── The_Beautiful_Cure--美しき免疫の力/
│   └── Siddhartha_Mukherjee/
│       ├── AUTHOR.md      # 著者情報統合ファイル
│       └── The_Song_of_the_Cell--細胞の歌/
└── ECONOMY/               # 経済学
    ├── Alvin_Roth/
    │   ├── AUTHOR.md      # 著者情報統合ファイル
    │   └── Who_Gets_What--誰が何を手に入れるのか/
    ├── Ariel_Rubinstein/
    │   ├── AUTHOR.md      # 著者情報統合ファイル
    │   └── Economic_Fables--ルービンシュタイン_ゲーム理論の力/
    └── von_Neumann_Morgenstern/
        ├── AUTHOR.md      # 著者情報統合ファイル
        └── Theory_of_Games_and_Economic_Behavior--ゲームの理論と経済行動/
```

## 機能と特徴

### 著者別分類システム
- **著者ディレクトリ**: 各著者の全著作を一箇所に整理
- **AUTHOR.md**: 著者の包括的情報（経歴、貢献、主要著作）
- **書籍固有の著者ファイル**: その書籍執筆前後の特筆すべき情報

### 分野別分類
- **BIOLOGY**: 生物学・生命科学関連の書籍
- **ECONOMY**: 経済学・ゲーム理論関連の書籍
- 今後追加予定: PHYSICS（物理学）、CHEMISTRY（化学）など

### 二言語対応
- **英語版（en/）**: 原著の章タイトルと科学用語
- **日本語版（jp/）**: 日本語翻訳版の要約とローカライズされた内容

### 構造化されたコンテンツ
各章ファイルの構成：
- **章の概要**: 主要テーマの簡潔な要約
- **主な内容**: 重要トピックの詳細な箇条書き
- **重要なポイント**: 必須の要点と概念

## 使い方

### 読書用
1. 著者ディレクトリの `AUTHOR.md` で著者の全体像を把握
2. `全体構成.md` で書籍全体の概要を理解
3. `著者_[名前].md` でその書籍執筆時期の背景を確認  
4. 章ファイルを順次読み進める、または関心のある章から
5. `読書メモ.md` で個人的な所感を記録

### 研究用
- 章を横断してトピック検索
- 二言語コンテンツで用語の対照
- 著者情報と書籍構造の参照
- 読書進捗と洞察の追跡

### 拡張用
新しい書籍を追加する際の手順：
1. 適切な分野ディレクトリに書籍フォルダを作成
2. 確立された構造に従ってファイル作成
3. 二言語の一貫性を維持
4. このREADMEを新しい追加内容で更新

## ファイル命名規則
- **書籍**: `Title--Japanese_Title/`
- **著者**: `Author_FirstnameLastname.md` / `著者_[名前].md`
- **章**: `Chapter[N]_Title.md` / `第[N]章_タイトル.md`
- **部**: `Part[N]_Title/` / `第[N]部_タイトル/`

## 収録書籍

### BIOLOGY（生物学・生命科学）

#### Richard Dawkins (リチャード・ドーキンス)
- **The Selfish Gene (利己的な遺伝子)** - 遺伝子中心の進化論の古典
- **The Blind Watchmaker (盲目の時計職人)** - 創造論への反駁と自然選択の力

#### John Maynard Smith (ジョン・メイナード・スミス)
- **Evolution and the Theory of Games (進化とゲーム理論)** - 進化ゲーム理論の基礎

#### Daniel M. Davis (ダニエル・M・デイヴィス)
- **The Beautiful Cure (美しき免疫の力)** - 現代免疫学の革命と医学的応用

#### Siddhartha Mukherjee (シッダールタ・ムカジー)
- **The Song of the Cell (細胞の歌)** - 細胞生物学の発見史から現代医療まで

### ECONOMY（経済学）

#### Alvin E. Roth (アルビン・E・ロス)
- **Who Gets What — and Why (誰が何を手に入れるのか)** - マーケットデザインとマッチング理論

#### Ariel Rubinstein (アリエル・ルービンシュタイン)
- **Economic Fables (ゲーム理論の力)** - ゲーム理論の批判的検討と経済モデルの限界

#### John von Neumann & Oskar Morgenstern (フォン・ノイマン&モルゲンシュテルン)
- **Theory of Games and Economic Behavior (ゲームの理論と経済行動)** - ゲーム理論の古典的基礎

## ライセンス

このプロジェクトは個人的な読書記録のためのものです。書籍の内容に関する著作権は各著者および出版社に帰属します。