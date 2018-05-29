# mongodb-mongohacker

## version
mongodb 3.7.9
mongohacker 0.0.10

## to create container without name
docker run -p 27017:27017 -d pedrualves/mongodb-mongohacker

## to access container without name
docke exec -it <id or custom name> mongo

## to create container with name
docker run --name mongo-maneiro -p 27017:27017 -d pedrualves/mongodb-mongohacker

## to access container with name
docke exec -it mongo-maneiro mongo
