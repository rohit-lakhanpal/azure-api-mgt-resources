# azure-api-mgt-resources
This repository contains all relevant assets required to follow the "Azure API Management" series of blog posts at https://devtasks.blogspot.com/2017/05/azure-api-management.html

# getting started
You can host the contents of the db.json file using the following commands (assuming you have nodejs/npm installed)
> npm install -g json-server

> npm install -g bootprint

> npm install -g bootprint-openapi

> bootprint openapi https://raw.githubusercontent.com/rohit-lakhanpal/azure-api-mgt-resources/master/swagger.json public

> wget https://raw.githubusercontent.com/rohit-lakhanpal/azure-api-mgt-resources/master/db.json

> json-server --port 8080 --watch db.json & disown

If all your pre-requisites are met, you should now be able to host apis based off the db.json. 
```
root@usw2-apidemo-server01:~# npm install -g json-server
...
root@usw2-apidemo-server01:~# npm install -g bootprint
...
root@usw2-apidemo-server01:~# npm install -g bootprint-openapi
...
root@usw2-apidemo-server01:~# wget https://raw.githubusercontent.com/rohit-lakhanpal/azure-api-mgt-resources/master/db.json
root@usw2-apidemo-server01:~# json-server --watch db.json --port 8080 & disown
[1] 22862
root@usw2-apidemo-server01:~#
  \{^_^}/ hi!

  Loading db.json
  Done

  Resources
  http://localhost:8080/posts
  http://localhost:8080/comments
  http://localhost:8080/albums
  http://localhost:8080/photos
  http://localhost:8080/users
  http://localhost:8080/todos

  Home
  http://localhost:8080

  Type s + enter at any time to create a snapshot of the database
  Watching...
```
