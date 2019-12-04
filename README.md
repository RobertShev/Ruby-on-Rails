# Ruby-on-Rails

##Guide

1. Download and install
* http://railsinstaller.org/en
* https://rubyinstaller.org/downloads/
2. open cmd/terminal as administrator
3. check is everything installed
* rails --version
* sqlite3 --version
6. gem install rails
7. rails new demoapp
8. cd demoapp
9. bundle install
10. gem install sqlite3 -v '1.4.1' --source 'https://rubygems.org/'
11. bundle install
12. Install yarn from  https://yarnpkg.com/lang/en/docs/install/
13. rails server
* http://localhost:3000 (port shown in terminal)
15. in config/routes.rb add
* root 'movies#index'
17. rails db:migrate
18. add validation in Demoapp/app/models/movie.rb
* validates :name, presence: true, uniqueness: true
* validates :descriptions, presence: true
21. Rails server to check changes
22. ADD authentication in App/controllers/application_controller.rb
* http_basic_authenticate_with name: 'admin', password: 'password', except: [:index, :show]
24. rails server
