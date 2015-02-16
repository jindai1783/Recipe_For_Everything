# Rails

1.
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
_Migrating the database in heroku_
```
heroku run rake db:migrate
```