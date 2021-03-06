
### Modeling Scrum Poker

![](https://raw.githubusercontent.com/valterbarros/scrum-poker/master/modeling_project/logic-model.png)

## Dependencies

* Ruby version 2.4.2
* Rails version 5.1
* Postgres >= 9.5

You must have redis installed and running on the default port:6379 (or configure it in config/redis/cable.yml).

### Installing Redis
##### On Linux
* `wget http://download.redis.io/redis-stable.tar.gz`
* `tar xvzf redis-stable.tar.gz`
* `cd redis-stable`
* `make`
* `make install`

##### On Mac
* `brew install redis`

###### Note: You must have Ruby 2.2.2 installed in order to use redis

## Starting the servers

1. bundle install
2. rake db:create && rake db:migrate
3. redis-server
4. rails s
5. Visit `http://localhost:3000`
