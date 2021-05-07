source "https://rubygems.org"

gem "inherited_resources", github: "user512/inherited_resources", branch: "rails-5-2-6"
gemspec

group :development, :test do
  gem "rake"
  gem "pry" # Easily debug from your console with `binding.pry`
  gem "pry-byebug", platform: :mri # Step-by-step debugging

  gem "cancancan"
  gem "pundit"
  gem "jruby-openssl", "~> 0.10.5", platform: :jruby

  gem "draper", "~> 4.0"
  gem "devise"

  gem "rails", "~> 6.1.0"
  gem "activerecord-jdbcsqlite3-adapter", "~> 61.a", github: "jruby/activerecord-jdbc-adapter", platform: :jruby

  gem "sprockets-rails"
  gem "sassc-rails", "~> 2.1"

  gem "formtastic", "~> 4.0.rc1"
end

group :test do
  gem "cuprite", "0.11"
  gem "capybara", "~> 3.14"
  gem "db-query-matchers", "0.10.0"

  gem "simplecov", "0.20.0", require: false # Test coverage generator. Go to /coverage/ after running tests
  gem "cucumber-rails", "~> 2.0", require: false
  gem "cucumber"
  gem "database_cleaner"
  gem "jasmine"
  gem "jasmine-core", "2.99.2" # last release with Ruby 2.2 support.
  gem "launchy"
  gem "parallel_tests", "~> 3.0"
  gem "rails-i18n" # Provides default i18n for many languages
  gem "rspec-rails"
  gem "sqlite3", "~> 1.4", platform: :mri
end

group :release do
  gem "chandler", "0.9.0" # Github releases from changelog
  gem "octokit", "~> 4.18"
end

group :lint do
  # Code style
  gem "rubocop", "0.93.1"
  gem "rubocop-packaging", "0.5.1"
  gem "rubocop-rspec", "~> 1.30"
  gem "rubocop-rails", "~> 2.3"
  gem "mdl", "0.11.0"

  # Translations
  gem "i18n-tasks"
  gem "i18n-spec"
end

group :docs do
  gem "yard" # Documentation generator
  gem "kramdown" # Markdown implementation (for yard)
end

gemspec path: "."
