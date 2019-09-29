# simple-nodejs-dockerfile
#### $docker build . -t mynodejs:1.0
#### $docker run -d --name mynodejs-container -p 3000:3000 -e DATABASE_USER=admin -e DATABASE_PASSWORD=1111 -e DATABASE_HOST=mymongodb-container --network shoppers mynodejs:1.0

#### $docker build . -t mymongodb:1.0
#### $docker run -d --name mymongodb-container mymongodb:1.0

#### $docker logs mynodejs-container


#### docker build -f Dockerfile.prod . -t myreactapp:1.1
#### $docker run -p 3001:80 --network shoppers -d --name myreactapp_prod myreactapp:1.1