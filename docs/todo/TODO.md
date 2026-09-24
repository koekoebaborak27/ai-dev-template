# TODO

<PROJECT_NAME> の**残タスクと現在地**。

**このファイルには「いま何が残っているか」だけを書く。** 設計・手順・経緯は下表の担当ファイルへ書き、ここからはリンクするだけにする。同じ内容を 2 か所に置かない。**150 行を超えたら、抱え込んでいる内容を担当ファイルへ移す。**

| 書きたいこと | 書く場所 |
| --- | --- |
| **残タスク・進捗・次の一手** | **このファイル** |
| 要件・設計・仕様の決定 | [`docs/specs/`](../specs/README.md) |
| 本番構築の手順・本番構成・環境変数 | [`docs/specs/99_infra/`](../specs/99_infra/README.md) |
| 設定値・落とし穴・実測値 | [`docs/todo/notes/`](notes/README.md) |
| 何をやったか・なぜ・どこで詰まったか | [`docs/todo/history/`](history/README.md)（古い順。新しい記録は末尾へ） |
| 開発フロー | [`docs/development/gitの操作ルール.md`](../development/gitの操作ルール.md) |
| 初めて触る人が必要とする情報 | [`README.md`](../../README.md) |

このファイルの更新手順は [`docs/skills/update-todo.md`](../skills/update-todo.md)（`/update-todo` の正本）。

## 進捗サマリ

**進捗を書くのはこの表だけ。** 他の節に「N / M 完了」を重ねて書かない。

| 区分 | 進捗 |
| --- | --- |
| <区分名> | 0 / 0 |

## 次にやること

**次のセッションが最初に打つコマンドまで具体的に書く。**

```powershell
git log --oneline -1     # 現在のコミット
git status --porcelain   # 未コミット差分がないか確認
```

- [ ] 1. 要件定義（→ [`docs/specs/`](../specs/README.md)）
- [ ] 2. 画面イメージ検討（必要かどうかを判断する。必要な場合は検討者が画像を用意してAIへ渡し、[`DESIGN.md`](../../DESIGN.md) の内容を刷新する）
- [ ] 3. 基本設計（要件定義で定まっていない部分のみ。→ [`docs/specs/`](../specs/README.md)）
- [ ] 4. 詳細設計（基本的には不要。基本設計で定まっていない部分のみ）
- [ ] 5. 実装・単体ロジックテスト（1機能ずつ実装する。→ [`create-vitest-test`](../skills/create-vitest-test.md)）
- [ ] 6. 画面テスト（必要かどうかを判断する。必要な場合は [`create-unit-test-spec`](../skills/create-unit-test-spec.md) でテスト仕様書を作成したうえで [`playwright-evidence-test`](../skills/playwright-evidence-test.md) を行う）
- [ ] 7. ユーザテスト（必要かどうかを判断する）

## 残っているタスク

いずれも**期限のない宿題**。判断材料は各リンク先にまとめる。

- [ ] <いつかやること>

## 現在の状態

事実のみ。予定・経緯・仕様は書かない。

| 項目 | 状態 |
| --- | --- |
| 作業ブランチ | `main` |
| ローカル環境 | <未構築 / 構築済み> |
| 本番 | <未構築 / 稼働中> |

## 完了済みの作業

各区分の実施内容・判断・詰まった点は [`docs/todo/history/`](history/README.md) にセッション単位で残す。

| 区分 | 件数 | 記録 |
| --- | --- | --- |
| <区分名> | 0 | — |
