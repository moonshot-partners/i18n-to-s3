source "https://rubygems.org"

gem "jets"

# to push translated files to S3
gem 'aws-sdk-s3', '~> 1'

# to get base file from repository
gem "octokit", "~> 4.18.0"

# to translate keys
gem "google-cloud-translate", "~> 1.3.0", require: "google/cloud/translate"

# to update existing files
gem "hashdiff", "~> 1.0.1"

# Parse and format i18n messages using ICU MessageFormat
gem 'message_format'

# development and test groups are not bundled as part of the deployment
group :development, :test do
  # Call 'byebug' anywhere in the code to stop execution and get a debugger console
  gem 'byebug', platforms: [:mri, :mingw, :x64_mingw]
  gem 'shotgun'
  gem 'rack'
  gem 'puma'
  gem 'pry', '~> 0.12.2'
end

group :test do
  gem 'rspec' # rspec test group only or we get the "irb: warn: can't alias context from irb_context warning" when starting jets console
  gem 'launchy'
  gem 'capybara'
end
