# テーブル設計
## usersテーブル

| column   | type   | option     |
|----------|--------|------------|
| email    | string | null:false |
| password | string | null:false |
| name     | string | null:false |
| profile  | text   | null:false |
| position | text   | null:false |

## prototypesテーブル

| column     | type      | option        |
|------------|-----------|---------------|
| title      | string    | null:false    |
| catch_copy | text      | null:false    |
| concept    | text      | null:false    |
| image      | -         | ActiveStorage |
| user       | reference | -             |

## commentsテーブル
| column     | type      | option        |
|------------|-----------|---------------|
| text       | text      | null:false    |
| user       | reference | -             |
| prototype  | reference | -             |