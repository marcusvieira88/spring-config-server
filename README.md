# Introduction

This microservice is a example of how implement a spring config server that stores the configs in a Redis database.

# Start

First, you need to run the docker-compose to create the redis database:

```
docker-compose up
```

Then you can use the redis-cli tool for connect to Redis database:

```
redis-cli
``` 

Insert some test keys in the database, for example:

```
HMSET spring-config-microservice config "Config Redis" configb "Config B Redis"
```
Example with application name and profile dev:

```
HMSET spring-config-microservice-dev config "Config Redis Dev" configb "Config Redis B Dev"
```