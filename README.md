Based on Calendar example app by RichOnRails.com.  See http://richonrails.com/articles/building-a-basic-calendar-in-ruby-on-rails for details.

Adaptation done:

- gemfile: change sqlite3 to postgresql (switch gem 'sqlite3' to 'pg')
- use `bundle update` instead of `bundle install` (which solved the issue of `gem install json -v '1.8.1'` error)
- replace database.yml with one that uses postgresql
