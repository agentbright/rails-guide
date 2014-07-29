rails-guide
===========

Create new application
Add postgres database
Install gems
Devise
Foundation
Active Admin
jquery-ui-rails
simple_form
jquery-turbolinks



### Project - Create IT Capabilities Application

1. Create app
2. Create git repo
3. Clone to local
4. Create new rails app
5. Make sure it runs
6. Add postgresql
  - Add ‘gem pg’ to the gemfile
  - Add .pgapp settings file
  - remove ‘development.sqllite3
  - Run rake db:create
  - Run rake db:migrate

7. Add the following gems
- jquery-ui-rails - https://github.com/joliss/jquery-ui-rails
  - add to application.js and application .css
- simple_form
  - Add simple_form gem
  - DON’T RUN THE GENERATOR YET
  - Add country_select gem
- jquery-turbolinks - https://github.com/kossnocorp/jquery.turbolinks
  - Install gem
  - add to application.js
- devise - https://github.com/plataformatec/devise
  - Install gem
  - run installer
  - generate devise model ‘User’
  - rake db:migrate
  - Install devise_security_extension - https://github.com/phatworx/devise_security_extension
- active admin - http://activeadmin.info/
  - INstall active admin 1.0.0 gem
  - Run active admin installer
- Add settings.yml file
- Add setup.rake to lib/tasks
  - https://gist.github.com/heyogrady/8d20b466da7471159808
- Install Foundation
  - Add gem foundation-rails
  - Inside group :development, add
  `gem rails_layout`
  - Run rails layout generator
  `rails generate layout:install foundation5 --force`
  - Run simple_form generator
  `rails generate simple_form:install --foundation`
