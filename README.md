# テーブル設計

## users テーブル

| Column     | Type   | Options     |
| --------   | ------ | ----------- |
| email      | string | not null    |
| password   | string | not null    |
| name       | string | not null    |
| profile    | text   | not null    |
| occupation | text   | not null    |
| position   | text   | not null    |

### Association



## prototypes テーブル

| Column     | Type   | Options     |
| ------     | ------ | ----------- |
| title      | string | not null    |
| catch_copy | text   | not null    |
| concept    | text   | not null    |
| user       | references           |

### Association



## comments テーブル
| Column     | Type   | Options     |
| ------     | ------ | ----------- |
| text       | text   | not null    |
| user       | references           | 
| prototype  | references           |

### Association