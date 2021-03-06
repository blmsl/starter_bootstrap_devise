[![Code Climate](https://codeclimate.com/github/jason-hobbs/starter_bootstrap_devise/badges/gpa.svg)](https://codeclimate.com/github/jason-hobbs/starter_bootstrap_devise) [![Test Coverage](https://codeclimate.com/github/jason-hobbs/starter_bootstrap_devise/badges/coverage.svg)](https://codeclimate.com/github/jason-hobbs/starter_bootstrap_devise/coverage)
[![security](https://hakiri.io/github/jason-hobbs/starter_bootstrap_devise/master.svg)](https://hakiri.io/github/jason-hobbs/starter_bootstrap_devise/master)
[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)

###Starter_Bootstrap

This is a starter site for Ruby on Rails apps.  
It has bootstrap 4 beta, gritter notifications, postgresql, gravatar, and devise built in.  
Uses Ruby 2.4.2 and Rails 5.1.3
[Demo here](http://starter-bootstrap-devise.herokuapp.com).  

Clone to a folder, then:  
&nbsp;&nbsp;Create a file in the root of the folder named: .env  
&nbsp;&nbsp;copy and paste the following with any changes you want:  

```
  DATABASE_USER=user
  DATABASE_PASSWORD=password
  DEV_DATABASE_NAME=starter_bootstrap_dev
  TEST_DATABASE_NAME=starter_bootstrap_test
  DATABASE_NAME=starter_bootstrap
  GMAIL_USERNAME=user@gmail.com
  GMAIL_PASSWORD=password
```
Then run:

```
bundle
rails db:setup
```

Look at db/seeds.rb for the default user and admin logins.

Run:
```
rspec
```
to run all tests.

Then just add your own Models, Views, and Controllers!


Password confirmation, reset, and unlock is sent using Gmail.  To use Mandrill, Mailgun, etc. just
edit the config/environments/development.rb and production.rb changing the
settings in config.action_mailer.smtp_settings.
