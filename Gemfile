source 'https://rubygems.org'

gem 'rails', '4.0.0.beta1'

# Gems used only for assets and not required
# in production environments by default.
group :assets do
  gem 'sass-rails',   '~> 4.0.0.beta1'
  gem 'coffee-rails', '~> 4.0.0.beta1'

  gem 'uglifier', '>= 1.0.3'
end

group :development do
  gem 'thin'

  gem 'guard'
  # Filesystem API
    gem 'rb-inotify', require: false # Linux
    gem 'rb-fsevent', require: false # OSX
    gem 'rb-fchange', require: false # Windows
  # Notification API
    gem 'ruby_gntp', require: false # Windows / OSX

  gem 'guard-bundler'
  gem 'guard-migrate'
  gem 'guard-rails'
  gem 'guard-rspec'
  # FIXME: Jasmine blocked
  #gem 'guard-jasmine'
end

group :test do
  gem 'capybara'
  gem 'poltergeist', git: 'git://github.com/jonleighton/poltergeist.git'
  gem 'phantomjs', require:'phantomjs/poltergeist'
  gem 'launchy' # Allows capybara to open a browser
end

group :test, :development do
  # Testing tools
  gem 'rspec-rails', '~> 2.0'
  # FIXME: Internal routes currently broken in Rails 4
  # gem "jasminerice"

  # Debug
  gem 'pry'
  gem 'traceroute'
end

# Custom Groups
#
# See: http://iain.nl/getting-the-most-out-of-bundler-groups
group :datastores do
  gem 'sqlite3'
end

group :ui_frameworks do
  gem 'jquery-rails'
  gem 'haml-rails'
  gem 'twitter-bootstrap-rails'
  # FIXME: No Rails 4 fork yet
  #gem "rails-backbone"
end

group :security do
  # TODO: Move to released versions ASAP
  gem 'devise', git: 'git://github.com/plataformatec/devise.git', branch: 'rails4'
  # TODO: Drop this when devise supported Strong Params
  gem 'protected_attributes'
end

group :analytics do
  gem 'google-analytics-rails'
end

group :file_uploads do
  # TODO: Don't need this just yet
  #gem 'rmagick'
  gem 'carrierwave'
end

group :forms do
  # TODO: Don't need this just yet
  #gem 'mail_form'
  gem 'client_side_validations'
end

# TODO: No Rails 4 fork for ActiveAdmin yet
group :backoffice do
  #gem 'activeadmin'
  #gem 'active_admin_sortable', git: "git://github.com/krhorst/active_admin_sortable.git"
  #gem 'active_admin_editor'
end

group :rails_ext do
  # Humanized urls
  gem 'friendly_id'
  # Simple single-file config helper
  gem 'rails_settings', git: 'git://github.com/brrygrdn/rails_settings.git'
end

# Additional Rails 4 defaults
#
# TODO: Determine if we need these....
group :misc do
  # Turbolinks makes following links in your web application faster. Read more: https://github.com/rails/turbolinks
  gem 'turbolinks'

  # Build JSON APIs with ease. Read more: https://github.com/rails/jbuilder
  gem 'jbuilder', '~> 1.0.1'
end


