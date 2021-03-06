# Phprest Sample Heroku App

[![Author](http://img.shields.io/badge/author-@adammbalogh-blue.svg?style=flat-square)](https://twitter.com/adammbalogh)
[![Software License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square)](LICENSE)

# Demo

[phprest.herokuapp.com/docs](http://phprest.herokuapp.com/docs)

# Api docs screenshot

![Api docs](http://i.imgur.com/OZVO8eF.png)

Of course you can send curl requests too:

```cli
curl -X GET --header "Accept: */*" phprest.herokuapp.com/camera
```

# Installation

* Install [Heroku Toolbelt](https://toolbelt.heroku.com)
* ```heroku login```
* ```heroku create yourappname```
* ```heroku addons:add --app yourappname cleardb:ignite```
* ```git clone https://github.com/phprest/phprest-sample-heroku-app.git```
* ```cd phprest-sample-heroku-app```
* ```heroku git:remote -a yourappname```
* ```git push heroku master```
* ```heroku run bash```
 * ```vendor/bin/phprest-service-orm migrations:migrate```
 * ```vendor/bin/phprest-service-orm fixtures:set```

