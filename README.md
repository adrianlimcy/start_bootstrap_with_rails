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

Notes:
To use images in the bootstrap scss, remember to change the scss to scss.erb,
then remember to change any background image from
background-image: url("../img/header-bg.jpg");
to
background-image: url(<%= asset_path 'header-bg.jpg' %>);

fixed the font-awesome issue by installing the gem 'font-awesome-rails'
simplified things by installing the gem 'bootstrap'

used @import "jquery-ui/core" @import "jquery-ui/theme" in the application.sass

added the cdn link in application.html.erb for jquery easing since the gem didn't have it
added the <%= javascript_include_tag 'agency' %> to include the js

Put all the js files into vendor/assets/javascript/
had an error
ActionView::Template::Error (Asset was not declared to be precompiled in production.
Add `Rails.application.config.assets.precompile += %w( agency.js )` to `config/initializers/assets.rb` and restart your server):
so did what it advised
