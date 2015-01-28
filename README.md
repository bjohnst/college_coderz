# Fork Me!

## Installation Notes

[Ruby on Rails](http://rubyonrails.org/) application backed by [PostgreSQL](http://www.postgresql.org/). Matrix is being developed against Ruby 2.1.4. The Rails environment for this application is 4.1.8.

PostgreSQL can be obtained for all versions of operating systems, however, for *nix style environments this is easiest through your package manager; i.e. `apt-get install postgresql` _or_ `brew install postgresql`. Once PostgreSQL is installed, you will need to create a user for the application with `sudo -u postgres createuser --createdb --pwprompt <desired_username>` which will prompt for the desired password. As PostgreSQL requires users creating databases to also be system users, you can either use your existing system account for this, or also create this user in your system.

### Startup

* Install necessary Gems
  * `cd path/to/app`
  * `bundle install`
* Setup database config ( _only on first run_ )
  * `config/database.yml`
  * Edit credentials for your PG user
* Start the server
  * `rails s`

