# frozen_string_literal: true

source "https://rubygems.org"

ruby RUBY_VERSION
DECIDIM_VERSION={:github => "Platoniq/decidim", :branch => "master"}

gem "decidim", DECIDIM_VERSION
# gem "decidim-consultations", DECIDIM_VERSION
# gem "decidim-initiatives", DECIDIM_VERSION

gem "bootsnap", "~> 1.3"

gem "puma", "~> 3.12.2"
gem "uglifier", "~> 4.1"

gem "faker", "~> 1.9"
gem "health_check"
gem "sidekiq", "~> 5.2"
gem "sidekiq-cron"
gem "sentry-raven"
gem "rspec"

group :development, :test do
  gem "byebug", "~> 11.0", platform: :mri

  gem "decidim-dev", DECIDIM_VERSION
end

group :development do
  gem "letter_opener_web", "~> 1.3"
  gem "listen", "~> 3.1"
  gem "spring", "~> 2.0"
  gem "spring-watcher-listen", "~> 2.0"
  gem "web-console", "~> 3.5"
end

group :production do
  gem "fog-aws"
end
