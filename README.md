# Dice.io Heroku application

A simple example to deploy you own dice.io server on Heroku.

## Getting started

This document assume that :

* [Heroku CLI](https://devcenter.heroku.com/articles/heroku-command-line) is installed
* You are logged in to you Heroku account (ie: `heroku login`)
* You have created an application. For example `my-app-name`

Clone this repository :

```shell
$ git clone https://github.com/tpftg/diceio-heroku.git
cd diceio-heroku
```

Add `my-app-name` Heroku remote branch :

```shell
$ heroku git:remote -a my-app-name
```

Deploy your application :

```shell
$ git push heroku master
```

When deployment ends demo application should be available, for example, at `https://my-app-name.herokuapp.com`.

It is recommended to enable session affinity :

```shell
$ heroku features:enable http-session-affinity
```
