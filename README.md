# テーブル設計

## users テーブル

| Column   | Type   | Options     |
| -------- | ------ | ----------- |
| email    | string |             |
| password | string |             |
| name     | string |             |
| profile  |  text  |             |
|occupation|  text  |             |
| position |  text  |             |
## protoypes テーブル

|  Column  | Type     | Options     |
| -------- | -------- | ----------- |
|   title  | string   | null: false |
|catch_copy|  text    |             |
|  concept | text     |             |
|  image   |          |             |
|  user    |references|             |
## comments テーブル

| Column  | Type       | Options                        |
| ------- | ---------- | ------------------------------ |
|   text  | text       |                                |
|  user   | references | null: false, foreign_key: true |
|prototype| references | null: false, foreign_key: true |



