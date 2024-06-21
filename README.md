予定を入力・確認できるシンプルなカレンダーアプリ開発中

【6/20】
画面遷移図・データベース設計及びER図構築中

# userテーブル

| Column | Type     | Options     |
| ------ | -------- | ----------- |
| name   | string   | null: false |

# scheduleテーブル
| Column      | Type       | Options     |
| ----------- | ---------- | ----------- |
| title       | string     | null: false |
| category_id | string     | null: false |
| data        | data       | null: false |
| time        | time       |  |
| content     | text       |  |
| user_id     | references | null: false, foreign_key: true |

