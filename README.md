# DB設計



## categoriesテーブル

| Column | Type   | Options     |
| ------ | ------ | ----------- |
| name   | string | null: false |

### Association
- has_many :ideas



## ideasテーブル

| Column      | Type       | Options           |
| ----------- | ---------- | ----------------- |
| body        | text       | null: false       |
| category_id | references | foreign_key: true |

### Association
- belongs_to :category