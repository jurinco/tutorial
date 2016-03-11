# Ruby and Rails Tutorial Application

[Ruby On Rails Tutorial](http://railstutorial.org) by [OSD](http://osdglobal.com)


ERROR - Could not load 'guard/rspec' or' ' find class Guard::Rspec

This error spent a more hours, and i found true way

$ cd <appfolder>
$ vim Gemfile

instead of 
gem 'guard-rspec', '2.5.0'
replace on
gem 'guard-rspec', '4.6.0'


instead of 
gem 'rspec-rails', '2.13.1'
replace on
gem 'rspec-rails', '3.3.2'

And

$ bundle update
$ bundle exec guard init rspec