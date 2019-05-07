
*Make sure redis server is reachable, cmd: **redis-server***

## Redis install

```js
//https://www.npmjs.com/package/redis
npm i redis
```

## Setup

```js


const redis = require("redis");
const redisClient = redis.createClient({
  // Set the host, (default to localhost). Mandatory for docker
  host: /REDIS_HOST/
});

```

## Docker compose service
```yml

redis:
  #https://hub.docker.com/_/redis
  image: redis
  ports:   
    - "6379:6379" #default redis server port

```



