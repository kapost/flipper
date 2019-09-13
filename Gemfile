source 'https://rubygems.org'
gemspec name: 'flipper'

Dir['flipper-*.gemspec'].each do |gemspec|
  plugin = gemspec.scan(/flipper-(.*)\.gemspec/).flatten.first
  gemspec(name: "flipper-#{plugin}", development_group: plugin)
end

gem 'pry'
gem 'rake', '~> 12.3.3'
gem 'shotgun', '~> 0.9'
gem 'statsd-ruby', '~> 1.2.1'
gem 'rspec', '~> 3.0'
gem 'rack-test', '~> 0.6.3'
gem 'sqlite3', "~> #{ENV['SQLITE3_VERSION'] || '1.3.11'}"
gem 'rails', "~> #{ENV['RAILS_VERSION'] || '6.0.0'}"
gem 'minitest', '~> 5.8'
gem 'minitest-documentation'
gem 'rubocop'
gem 'rubocop-rspec'
gem 'webmock', '~> 3.0'

group(:guard) do
  gem 'guard', '~> 2.15'
  gem 'guard-rubocop', '~> 1.3'
  gem 'guard-rspec', '~> 4.5'
  gem 'guard-bundler', '~> 2.2'
  gem 'guard-coffeescript', '~> 2.0'
  gem 'guard-sass', '~> 1.6'
  gem 'rb-fsevent', '~> 0.9'
end
