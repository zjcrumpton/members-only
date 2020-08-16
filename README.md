# README

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

We need 
    * users - username and password
    * posts - title ad body

Table: posts
Model: Post
Columns and Validations
    title:string
    body:text [present, length]
Associations
    belongs_to :user

Table: users
Model: User
Columns and Validations
    username:string
    password:text [present, length]
Associations
    has_many :posts

