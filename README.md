# MONGODB & MONGOHACKER

## versions!
* mongodb 3.7.9-xenial (https://hub.docker.com/r/library/mongo/)
* mongohacker 0.0.10 (https://github.com/TylerBrock/mongo-hacker)

## create container without name
docker run -p 27017:27017 -d pedrualves/mongodb-mongohacker

## access container without name
docker exec -it <id or custom name> mongo

## create container with name
docker run --name mongo-maneiro -p 27017:27017 -d pedrualves/mongodb-mongohacker

## access container with name
docker exec -it mongo-maneiro mongo
