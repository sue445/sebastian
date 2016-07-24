source "https://rubygems.org"

ruby "2.3.1"

# Distribute your app as a gem
# gemspec

# Server requirements
# gem 'thin' # or mongrel
# gem 'trinidad', :platform => 'jruby'

# Optional JSON codec (faster performance)
# gem 'oj'

# Project requirements
gem "rake"

# Component requirements
gem "sass"
gem "slim"
gem "activerecord", ">= 3.1", require: "active_record"

# Test requirements
gem "rspec", group: "test"
gem "rack-test", require: "rack/test", group: "test"

# Padrino Stable Gem
gem "padrino", "0.13.2"

# Or Padrino Edge
# gem 'padrino', :github => 'padrino/padrino-framework'

# Or Individual Gems
# %w(core support gen helpers cache mailer admin).each do |g|
#   gem 'padrino-' + g, '0.12.4'
# end

gem "actionpack", "~> 4.2.7"
gem "activerecord-import", "0.7.0"
gem "activerecord-simple_index_name"
gem "dalli"
gem "kaminari", require: "kaminari/sinatra"
gem "newrelic_rpm"
gem "rollbar"
gem "rroonga"
gem "sinatra", ">= 1.4.6"

group :development do
  gem "annotate"
  gem "dotenv", group: :test
  gem "foreman"
  gem "rubocop", "0.36.0"
  gem "sqlite3", group: :test
end

group :test do
  gem "coveralls", require: false
  gem "database_rewinder"
  gem "factory_girl"
  gem "faker-precure"
  gem "rspec-its"
  gem "rspec-padrino"
  gem "rspec-power_assert"
  gem "webmock"
end

group :production do
  gem "pg", group: :test
  gem "puma", group: :development
end
