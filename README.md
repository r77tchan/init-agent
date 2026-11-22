# init-agent

AIエージェントと協働するためのプロジェクト雛形。ルールを書いた `AGENTS.md`、次のセッションに渡すことを書く `doc/引き継ぎ.md`、永続メモリを切る設定が入る。

## 使い方

空のフォルダ（空のリポジトリでもよい）で実行する。この README 以外のファイルが、その場に置かれる。空でないときは、何もせずに止まる。

```sh
if [ -z "$(ls -A | grep -vxF -e .git -e .DS_Store)" ]; then curl -sL https://github.com/r77tchan/init-agent/archive/main.tar.gz | tar -xzk --strip-components=1 --exclude README.md; else echo "空のフォルダではないので、何もしなかった"; fi
```

そのあと、`AGENTS.md` の先頭にプロジェクトの説明を1行書く。

## AIに頼む場合

空のフォルダで、次のように伝える。

```text
https://github.com/r77tchan/init-agent の使い方どおりに、このフォルダを初期化して
```
