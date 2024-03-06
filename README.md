# Welcome to redis playground
## Install redis with docker 
    docker run -d --name redis-stack -p 6379:6379 -p 8001:8001 redis/redis-stack:latest
## Execute Docker command
    docker exec -it e78fc02789de bash
## Ping to redis
    redis-cli ping
## Go to redis CLI
    redis-cli
## Work on Redis
    set name Dilesh
    get name
    set user:1 Dilesh
    set user:2 Deepak
    set user:3 Dipti
    get user:1
    set user:1 Hello nx //It will not set if the key is already there 
    mget user:1 user:2 //To fetch multiple users