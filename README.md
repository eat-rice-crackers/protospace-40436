# README

# テーブル設計

## users テーブル

| Column             | Type   | Options      |
| ------------------ | ------ | -----------  |
| name               | string | null: false, |
| email              | string | null: false, unique: true |
| encrypted_password | string | null: false  |
| profile            | text   | null:false   |
| occupation         | text   | null:false   |
| position           | text   | null:false   |

## comments テーブル

| Column     | Type         | Options     |
| ------     | ------       | ----------- |
| content    | text         | null: false |
| prototype  | references   | null: false,  foreign_key: true |
| user       | references   | null: false,  foreign_key: true |


