# docker-sample-application

Following the docker tutorial

Currently at the [Part 8: Use Docker Compose](https://docs.docker.com/get-started/08_using_compose/), but the `docker-compose up` didn't start the application correctly with the following log entries:

```log
mysql_1  | Version: '5.7.33'  socket: '/var/run/mysqld/mysqld.sock'  port: 3306  MySQL Community Server (GPL)
app_1    | yarn install v1.22.5
app_1    | [1/4] Resolving packages...
app_1    | success Already up-to-date.
app_1    | Done in 0.19s.
app_1    | yarn run v1.22.5
app_1    | error Couldn't find a package.json file in "/app"
app_1    | info Visit https://yarnpkg.com/en/docs/cli/run for documentation about this command.
docker-sample-application_app_1 exited with code 1
```

But the file does appear to be in the `/app` folder.