# user_app (from sample_app)

__Great for rapid prototyping:__ fork this repo for simple way to have users all set up and get going on other models in rails. 

This is a clone of my [/sample_app](https://github.com/sample_app) that I wanted to put up, so you can quickly grab all the user requirements and start developing new models on top of it. This is the commit it was rolled back to: [commit](https://github.com/clamstew/sample_app/commit/2beeeec5196884aa8452672e9fd126e5740304f5) at the end of Chapter 9 exercises.

This is a modified version of the sample application for
[*Ruby on Rails Tutorial: Learn Rails by Example*](http://railstutorial.org/)
by [Michael Hartl](http://michaelhartl.com/).

This is where in the Rails Tutorial book you are at the point of this repo: [Beginning of Chapter 10](http://ruby.railstutorial.org/chapters/user-microposts#top).

This instance put together by [*Clay Stewart*](http://twitter.com/clay_stewart). Enjoy!

----------

In order to get this running you need to go into the <code>config/database.yml</code> file and change the __username__ to your computer (i.e. if you open up your finder and go to your home folder, __it should be the username at the top of the window next to the house icon on a mac__) user name. Then go into PostgreSQL by starting up the local Postgres application, and go to the elephant in your menubar, open "psql", and type <code>CREATE DATABASE user_app_development;</code> and <code>CREATE DATABASE user_app_testing;</code>. ([Here is some quick info on the PostgreSQL basics.](http://www.postgresql.org/docs/9.0/static/sql-createdatabase.html))

Then you have to run <code>$ bundle install</code>, <code>$ bundle exec rake db:migrate</code> in terminal to get it going.  Then you can run <code>$ rails s</code> and have the building blocks of a user based application.

I was using rspec for testing like Hartl. This was put together with the Rails 3.9.2 version of the book.