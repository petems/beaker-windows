# THIS REPO IS NOW DEPRECATED - Beaker and Beaker rspec now work with Windows Bitvise hosts without this fork.

To get a guarenteed working Windows + Beaker + Bitvise setup, the following in a Gemfile should work:

```ruby
group :system_tests do
  gem 'winrm', '1.8.1'
  gem 'beaker', '2.43.0'
  gem 'beaker-rspec', '5.3.0'
  gem 'beaker-puppet_install_helper',  :require => false
  gem 'vagrant-wrapper'
end
```
