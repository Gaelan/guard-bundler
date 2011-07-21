source 'http://rubygems.org'

gemspec

gem 'rake'

# optional development dependencies
require 'rbconfig'

if Config::CONFIG['target_os'] =~ /darwin/i
  gem 'rb-fsevent', '~> 0.4.0'
  gem 'growl',      '~> 1.0.3'
end
if Config::CONFIG['target_os'] =~ /linux/i
  gem 'rb-inotify', '~> 0.8.5'
  gem 'libnotify',  '~> 0.1.3'
end
if RbConfig::CONFIG['target_os'] =~ /mswin|mingw/i
  gem 'win32console',             :require => false
  gem 'rb-fchange',   '~> 0.0.2', :require => false
  gem 'rb-notifu',    '~> 0.0.4', :require => false
end
