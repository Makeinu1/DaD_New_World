# Claude Code での作業ガイド

このドキュメントは、Claude Code を使用してこのD&Dキャンペーンプロジェクトを編集・管理するためのガイドです。

## プロジェクト概要

このプロジェクトは、D&D 2024年版ルールを使用した自作キャンペーン「New World」の設計・管理用リポジトリです。
ボトムアップ方式（小さな村から世界を広げる手法）で構築されています。

## フォルダ構成

```
DaD_New_World/
├── CLAUDE.md              # このファイル - Claude Codeでの作業ガイド
├── README.md              # プロジェクト概要（一般向け）
├── .gitignore            # Git除外設定
├── campaign/             # キャンペーン全体の情報
│   ├── concept.md        # キャンペーンコンセプト
│   ├── world/            # 世界設定
│   │   ├── overview.md   # 世界の概要
│   │   └── timeline.md   # 年表
│   └── rules/            # ハウスルール・2024版活用
│       └── 2024-features.md
├── locations/            # 場所・地域
│   ├── starting-village/ # 初期拠点の村
│   │   ├── overview.md
│   │   └── npcs.md
│   └── regions/
├── npcs/                 # NPC情報
│   ├── allies.md
│   ├── villains.md
│   └── neutral.md
├── adventures/           # 冒険シナリオ
│   ├── session-01/
│   │   ├── overview.md
│   │   ├── encounters.md
│   │   └── rewards.md
│   └── hooks.md          # フック集
├── mechanics/            # ゲームメカニクス
│   ├── combat-encounters.md
│   ├── puzzles.md
│   └── skill-challenges.md
└── resources/            # リソース・参考資料
    ├── templates/
    └── references.md
```

## Claude Code での作業方法

### 新しいNPCの追加
```
適切なカテゴリ（allies/villains/neutral）のファイルに追加してください。
テンプレートは resources/templates/ にあります。
```

### 新しいセッションの準備
```
adventures/session-XX/ フォルダを作成し、
overview.md、encounters.md、rewards.md を作成してください。
```

### 場所の追加
```
locations/ 配下に新しいフォルダを作成し、
overview.md と npcs.md を作成してください。
```

## 編集のガイドライン

1. **マークダウン形式を使用**: すべてのドキュメントは `.md` 形式
2. **明確な見出し**: レベル2（##）から開始
3. **リンクの活用**: 関連するファイルへの相対リンクを活用
4. **テーブルの使用**: NPC統計やアイテムリストには表形式を推奨
5. **バージョン管理**: 大きな変更は適切なコミットメッセージで記録

## よく使うClaude Codeコマンド

- 新しいドキュメントの作成
- 既存ドキュメントの編集
- フォルダ構成の整理
- マークダウンのフォーマット修正
- 関連ファイル間のリンク作成

## 注意事項

- プレイヤーに見せたくない情報（ネタバレ、裏設定）には `[DM専用]` タグを付ける
- セッション後は `adventures/session-XX/notes.md` に実プレイの記録を追加
- NPCや場所の変更は、関連する全ファイルで整合性を保つ

## D&D 2024版の特徴的な要素

このキャンペーンでは、2024版の以下の新要素を積極的に活用します：
- 武器マスタリー（Weapon Mastery）
- 改訂されたスペル
- 新しいクラス機能
- 更新されたモンスター統計

詳細は [campaign/rules/2024-features.md](campaign/rules/2024-features.md) を参照してください。
