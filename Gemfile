source 'https://rubygems.org'

ruby "2.1.2"

# Bundle edge Rails instead: gem 'rails', github: 'rails/rails'
gem 'rails', '4.1.0'

# Use Devise for user authentication
gem 'devise', :git => 'git://github.com/plataformatec/devise.git', :ref => '49aebde'

# Use Omniauth for Authentication with Devise
gem 'omniauth'
gem 'omniauth-facebook'

# Use sqlite3 as the database for Active Record
gem 'sqlite3', :group => :development

gem 'haml'
gem 'haml-rails', :group => :development

# Use SCSS for stylesheets
gem 'sass-rails', '~> 4.0.0'

# Use Uglifier as compressor for JavaScript assets
gem 'uglifier', '>= 1.3.0'

# Use CoffeeScript for .js.coffee assets and views
gem 'coffee-rails', '~> 4.0.0'

# See https://github.com/sstephenson/execjs#readme for more supported runtimes
# gem 'therubyracer', platforms: :ruby


# Use jquery as the JavaScript library
gem 'jquery-rails'

# Use AWS for DynamoDB ActiveRecord substitute and S3 for file uploads
gem 'aws-sdk', '~> 2'

# FontAwesome
gem 'font-awesome-rails'

# Turbolinks makes following links in your web application faster. Read more: https://github.com/rails/turbolinks
gem 'turbolinks'

# Build JSON APIs with ease. Read more: https://github.com/rails/jbuilder
gem 'jbuilder', '~> 1.2'


gem 'paperclip', '~> 3.0'

# Twitter Bootstrap 3
gem 'anjlab-bootstrap-rails', :require => 'bootstrap-rails',
                              :github => 'anjlab/bootstrap-rails'

# Using puma for web server since this is faster on Heroku's Cedar Stack
gem 'puma'

group :production do
  gem 'pg'
end

group :development do
	gem 'factory_girl_rails'
	gem 'foreman' # For development since heroku already manages this with Procfile
end

group :doc do
  # bundle exec rake doc:rails generates the API under doc/api.
  gem 'sdoc', require: false
end

# Use ActiveModel has_secure_password
# gem 'bcrypt-ruby', '~> 3.0.0'

# Use unicorn as the app server
# gem 'unicorn'

# Use Capistrano for deployment
# gem 'capistrano', group: :development

# Use debugger
# gem 'debugger', group: [:development, :test]
