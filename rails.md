# Rails

## Inside the console

1.
_Initialisation_
```
rails new my_app
```

2.
```
bundle install --without production
```

3.
_Generating model_
```
rails generate scaffold User name:string email:string
```

```
rails g model restaurant name:string rating:integer
```

_Generating controller_
```
rails generate controller StaticPages home help
```

_Beware of 's'_
```
rails g controller restaurants
```

4.
_Migrating database_
```
bundle exec rake db:migrate
```

5.
```
rails server
```

6.
```
rails console
```

7.
_Migrating the database in heroku_ This is done after pushing the main contents to heroku.
```
heroku run rake db:migrate
```

8.
_Show built-in routes_
```
rake routes
```

9.
_Destroying a model_
```
rails d model restaurant
```

10.
_Test environment_
```
rake db:mirate RAILS_ENV=test
```

11.
_Migrating database_
```
rails g migration AddDescriptionToRestaurants description:text
```

12.
```
rails g migration AddRestaurantIdToReviews restaurant:belongs_to
```

## Inside the files

1.
_Model dependency_
```ruby
has_many :reviews, dependent: :destroy
```

```ruby
belongs_to :restaurant
```

2.
_Database auto-cleaning_
```ruby
config.use_transactional_fixtures = true
```