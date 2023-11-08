source "https://rubygems.org"
git_source(:github) { |repo| "https://github.com/#{repo}.git" }
ruby '3.1.2'
gem "rails", "~> 7.0.8"
gem "sqlite3", "~> 1.4"
gem "puma", "~> 5.0"
gem 'rswag'
gem "tzinfo-data", platforms: %i[ mingw mswin x64_mingw jruby ]
gem "bootsnap", require: false
group :development, :test do
  gem "debug", platforms: %i[ mri mingw x64_mingw ]
  gem "spring"
  gem 'rspec-rails', '~> 3.5'
end

gem 'unicorn', '~> 6.1.0'
gem 'pg', '~> 1.3.5'
gem 'sidekiq', '~> 6.4.2'
gem 'redis-rails', '~> 5.0.2'
