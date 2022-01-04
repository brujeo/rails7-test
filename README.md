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


* Changing DB to PostgresQL
rails db:system:change --to=postgresql
bundle
heroku run rake db:migrate

* Add Redis
heroku addons:create heroku-redis:hobby-dev -a mighty-tundra-27310

* Project Setup
git add .
heroku create
git push heroku main
bundle lock --add-platform x86_64-linux
git add Gemfile.lock
git commit -m "Added the platform"

** Project Live
https://stark-spire-67923.herokuapp.com/

