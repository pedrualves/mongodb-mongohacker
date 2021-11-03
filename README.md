# MONGODB & MONGOHACKER

## versions!
* mongodb:latest (https://hub.docker.com/r/library/mongo/)
* mongohacker 0.1.1 (https://github.com/TylerBrock/mongo-hacker)

## create container without name
docker run -p 27017:27017 -d pedrualves/mongodb-mongohacker

## access container without name
docker exec -it <id or custom name> mongo

## create container with name
docker run --name mongo-maneiro -p 27017:27017 -d pedrualves/mongodb-mongohacker

## access container with name
docker exec -it mongo-maneiro mongo

## importing dta
```cli
docker cp file.json mongo:/tmp/file.json
docker exec mongo mongoimport -d test -c collection --type json --file /tmp/file.json --jsonArray
