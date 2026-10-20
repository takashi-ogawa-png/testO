# docs — アプリに関するドキュメント

アプリに関する**人が読むドキュメント**を置く。KSD コマンドが読み書きするファイルの置き場所でもある。
配置の正本は `ksd_core/.ksd/steering/structure.md`「アプリ側ドキュメント」。

| ファイル | 誰が作るか | git |
|---|---|---|
| `AGENT_SPEC.md` | `/ksd:agent-discover`（利用可能エージェントの一覧） | **追跡する**（後段コマンドへの受け渡し資料） |
| `keycloak.md` | `/ksd:initialization`（admin へ `[keycloak]` Issue を申請し、払い出しの完了コメントを保存する）。client ID / realm / テストユーザーと**パスワードの Secret ID** | **追跡する**（平文の秘密を含まないため。パスワードの実値は Secret Manager にある） |
| その他（画面仕様・調査メモ・運用手順など） | 人 / コマンド | 内容に応じて |

- **要求仕様書はここに置かない。** 正本は `.ksd/specs/<feature>/requirement.md`（`/ksd:initialization` の生成物）。
- `/ksd:initialization` の事前資料の取り込みは `docs/*.md` を候補として探す（`AGENT_SPEC.md` だけは専用の工程が扱うため候補から除外される）。
