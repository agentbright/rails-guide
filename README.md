rails-guide
===========
- Create new application
- Add postgres database
- Install gems
- Devise
- Foundation
- Active Admin
- jquery-ui-rails
- simple_form
- jquery-turbolinks



### Project - Create IT Capabilities Application

2. Create git repo on github.com
  - http://monosnap.com/image/cMT442pwg5OaZbfRn4LsksKKfTTCNs
3. Clone to local
  - http://take.ms/ODD1t
4. Create new rails app
  - `rails new it-capabilities`
5. Make sure it runs
  - `bundle install`
  - `rails s`
6. Add postgresql
  - Remove the line `gem 'sqlite3'` from the gemfile
  - Add `gem 'pg'` to the gemfile
  - Add settings file
    - Add this file to the config folder - https://gist.github.com/heyogrady/450bc5868c0daed6c1df
    - Change the database names
    - Duplicate the file and remove the .pgapp from the end
  - remove ‘development.sqllite3` file
  - Run `rake db:create`
  - Run `rake db:migrate`

### Add the following gems

- **devise** - https://github.com/plataformatec/devise
  - Install gem
  - run installer - `rails generate devise:install`
  - Run `rails generate devise model User`
  - Run `rake db:migrate`
  - Install devise_security_extension - https://github.com/phatworx/devise_security_extension
    - Add gem
    - Run installer - `rails generate devise_security_extension:install`
- **simple_form**
  - Add simple_form gem
  - DON’T RUN THE GENERATOR YET
  - Add country_select gem
- Install Foundation
  - Add gem foundation-rails
  - Also add the rails_layout gem, but it should only be installed in the development environment. To do this, put it inside a :development group, like this:
  ```
  group :development do
    gem 'rails_layout'
  end
  ```
  - Run rails layout generator
  `rails generate layout:install foundation5 --force`
  - Run simple_form generator
  `rails generate simple_form:install --foundation`
- **jquery-ui-rails** - https://github.com/joliss/jquery-ui-rails
  - add to application.js and application .css
- **jquery-turbolinks** - https://github.com/kossnocorp/jquery.turbolinks
  - Install gem
  - add to application.js
- **active admin** - http://activeadmin.info/
  - INstall active admin 1.0.0 gem
  - Run active admin installer
- Add settings.yml file
- Add setup.rake to lib/tasks
  - https://gist.github.com/heyogrady/8d20b466da747115980
