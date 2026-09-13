# init-agent

AIエージェントと協働するためのプロジェクト雛形。

## 使い方

```sh
# 1. 始める
gh repo clone r77tchan/init-agent <new-name>

# 2. .gitとREADME削除
rm -rf .git README.md
```

## 構成

- `AGENTS.md` — セッション開始時に読むファイルの一覧
- `CLAUDE.md` — Claude Code 用（`AGENTS.md` を参照）
- `doc/指示.md` — プロジェクトのルールと目的（AIは編集しない）
- `doc/メモ.md` — セッションをまたいで残す情報の置き場
- `.claude/settings.json` / `.codex/config.toml` — 永続メモリ無効の設定
