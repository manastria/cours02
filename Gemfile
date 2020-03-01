# frozen_string_literal: true

source "https://rubygems.org"

git_source(:github) {|repo_name| "https://github.com/#{repo_name}" }

# gem "rails"
gem 'guard', '~> 2.16', '>= 2.16.1'
#gem 'guard-asciidoctor', '~> 0.1.1'
#gem 'rb-inotify', '~> 0.10.1'
gem 'guard-shell', '~> 0.7.1'
gem 'asciidoctor', '~> 2.0', '>= 2.0.10'
gem 'guard-livereload', '~> 2.5', '>= 2.5.2'
gem 'yajl-ruby', '~> 1.4', '>= 1.4.1'
gem 'eventmachine', '~> 1.2', '>= 1.2.7', :platforms => :ruby

# Obtenir la platform avec : bundle platform
platforms 'mswin', 'mingw', 'mswin64', 'x64_mingw' do
  gem 'tzinfo-data'

  group :test do
    gem 'wdm', '~> 0.1.1'
    gem 'win32console', '~> 1.3', '>= 1.3.2'
  end
end
