source 'http://ruby.taobao.org/'

def darwin_only(require_as)
  RUBY_PLATFORM.include?('darwin') && require_as
end

def linux_only(require_as)
  RUBY_PLATFORM.include?('linux') && require_as
end

gem 'rails', '4.1.12'
gem 'activerecord-deprecated_finders'
gem 'activerecord-session_store'
gem "nested_form"

# Specify a sprockets version due to security issue
# See https://groups.google.com/forum/#!topic/rubyonrails-security/doAVp0YaTqY
gem 'sprockets', '~> 2.12.3'

# tag runners
gem 'acts-as-taggable-on', '~> 3.4'

# DB
gem 'mysql2', group: :mysql
gem 'pg',     group: :postgres

# Settings
gem 'settingslogic'

# Web server
gem "unicorn", "~> 4.8.2"

# Haml
gem 'haml-rails','~> 0.5.3'

# Background jobs
gem 'slim'
gem 'sinatra', require: nil
gem 'sidekiq'

# Scheduled
gem 'whenever', require: false

# Format dates
gem 'stamp'

# Pagination
gem 'kaminari'

# State machine
gem 'state_machine'

# For API calls
gem 'httparty', '0.11.0'

# OAuth
gem 'oauth2', '1.0.0'

# API
gem 'grape'
gem 'grape-entity'
gem 'virtus', '1.0.1'

# Default values for AR models
gem "default_value_for", "~> 3.0.0"

# Slack integration
gem "slack-notifier", "~> 1.0.0"

# HipChat integration
gem 'hipchat', '~> 1.5.0'

# Encrypt variables
gem 'attr_encrypted', '1.3.4'

# Other
gem 'rake'
gem 'foreman'
gem 'jquery-rails', '~> 3.1.3'
gem 'gitlab_ci_meta', '~> 4.0'

gem 'sass-rails',   '~> 4.0.5'
gem 'coffee-rails', '~> 4.0.0'

gem 'uglifier', '>= 1.0.3'
gem 'bootstrap-sass', '~> 3.0'
gem "font-awesome-rails", '~> 3.2'
gem 'turbolinks'
gem 'jquery-turbolinks'
gem 'nprogress-rails'

# Soft deletion
gem "paranoia", "~> 2.0"

# Colored output to console
gem "colored"

# for aws storage
gem "fog", "~> 1.25.0"
gem "unf"


group :development do
  gem 'brakeman', require: false
  gem 'rack-mini-profiler', require: false
  gem 'annotate'
  gem 'quiet_assets'
  gem "letter_opener"
  gem "spring-commands-rspec"
end


group :development, :test do
  gem 'spring', '~> 1.3.6'
  gem 'minitest'
  gem 'pry'
  gem 'rspec-rails'
  gem 'capybara'
  gem 'poltergeist', '~> 1.5.1'
  gem 'factory_girl_rails'
  gem "ffaker"
  gem "byebug"
  gem "database_cleaner"
  gem 'shoulda-matchers'
  gem 'guard-rspec'
  gem 'rb-fsevent', require: darwin_only('rb-fsevent')
  gem 'growl',      require: darwin_only('growl')
  gem 'rb-inotify', require: linux_only('rb-inotify')

  gem "simplecov", require: false
  gem 'coveralls', '~> 0.8.2', require: false
  gem 'rubocop', '0.28.0', require: false
end

group :test do
  gem 'webmock'
  gem 'email_spec'
end
