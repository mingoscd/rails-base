# README

## How to Start project

The `runner` container is `shell` inside your app. It can be used to run (almost) everything: tests, migrations, Rake tasks, whatever. So it's not needed a new container every time I need to run a task.
We are going to setup the project dependencies here. Run

```
docker-compose run -rm runner
```

Once the shell is running.
Note: be is alias for `bundle exec`. You can define more alias in the `.dockerdev/.bashrc`


```
bundle i
be rails webpacker:install
be rails react_on_rails:install
```


