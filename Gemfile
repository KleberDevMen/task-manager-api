source 'https://rubygems.org'

git_source(:github) do |repo_name|
  repo_name = "#{repo_name}/#{repo_name}" unless repo_name.include?("/")
  "https://github.com/#{repo_name}.git"
end

gem 'rails', '~> 5.0.2'
gem 'pg', '~> 0.18'
gem 'puma', '~> 3.0'

group :development, :test do
  gem 'byebug', platform: :mri

  # Gens add
  gem 'rspec-rails', '~> 3.5'
  gem 'rubocop-rspec'
  gem 'devise' # autenticacao

end

group :test do

  # Gens add
  gem 'database_cleaner'
  gem 'shoulda-matchers', '~> 3.1' # escrever menos codigo no momento dos testes
  gem 'factory_bot_rails' # gerador de objetos
  gem 'faker' # dados ficticios
end

group :development do
  gem 'listen', '~> 3.0.5'
  gem 'spring'
  gem 'spring-watcher-listen', '~> 2.0.0'

  # Gens add
  gem 'spring-commands-rspec' # almenta a velocidade dos testes
end

gem 'tzinfo-data', platforms: [:mingw, :mswin, :x64_mingw, :jruby]
