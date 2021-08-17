# README

## users テーブル

| Column              | Type   | Options     　|
| ------------------  | ------ | ----------- 　|
| nickname            | string | null: false 　|
| profile             | text | null: false     |
| encrypted_password  | string | null: false 　|
| profile_image_id    | string | null: false 　|

### Association
has_many :items



## purchasesテーブル

| Column              | Type   | Options     |
| ------------------  | ------ | ----------- |
| user                | reference | foreign_key:true |
| title               | string | null: false 　|
| body                | text | null: false 　|
### Association
belongs_to :user





This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version

* System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...
