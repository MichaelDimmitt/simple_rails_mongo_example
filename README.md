# README

Application originated from article: https://blog.botreetechnologies.com/setting-up-ruby-on-rails-5-app-with-mongodb-in-10-minutes-3c400c055262;
they perform a linux information if you are not a mac user.

## Installation with mac:

```bash
brew install mongodb
# Follow instructions from homebrew for further install instructions.
brew services start mongodb
# Restart your computer.

bundle install 
rake db:create
open http://localhost:3000/articles
rails s
```

## commands implemented:
```bash
rails new my_mongo_app --skip-active-record

echo "gem 'mongoid', '~> 6.0'
gem 'bson_ext'" >> Gemfile

bundle install
rails g mongoid:config
rake db:create
rails g scaffold article name:string content:text

open http://localhost:3000/articles
rails s
```



