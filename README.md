# A simple boilerplate for a Rails app
Already included: 
- Rubocop and it's rules
- Configured RSpec
- Dockerfile and heroku.yml 
- Gems: slim, config, factory_bot_rails, faker, rails-controller-testing
- bootstrap 4.5.2

Ruby version:
ruby-2.7.1

## What to do to customize the app
- Rename the application: just find all occurences of 'this_repo' and change to your app title.
- Enable the railties that you need in config/application.rb

## Running application example
[Example of this app running on Heroku](https://this_repo.herokuapp.com/)

## Running locally
```
git clone https://github.com/mechos3d/this_repo
cd ./this_repo
bundle install 
rm -f ./config/credentials.yml.enc
bundle exec rails credentials:edit
docker build -t this_repo_image .
docker run --rm -e RAILS_ENV=production \ -p 3000:3000 --name=this_repo this_repo_image
```

## TODOS:
- tdb
- tdb
