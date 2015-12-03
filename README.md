# docker-vocbench

Quick and dirty docker compose to run vocbench. Clone this repository and run ```docker-compose up``` to start vocbench. Vocbench will be available on http://localhost:10140/vocbench, sesame workbench on http://localhost:1150/openrdf-workbench . VB has been preconfigured with an administrator user. Use following credentials to connect as administrator. Vocbench requires no user by default.

* Username: administrator
* Password: 111111


## Configuration
You will need to configure access to the mysql db, the sesame repository and semantic turkey. Find defaults below to get you going. Check https://aims-fao.atlassian.net/wiki/display/VB/Quick+Test+Drive to get started. 

```
CFG.DB.CONNECTIONURL = jdbc:mysql://mysql:3306/vocbench?requireSSL=false&amp;useUnicode=true&amp;characterEncoding=UTF-8
CFG.DB.USERNAME = vocbench
CFG.DB.PASSWORD = ieg9ohZi
Semantic Turkey Server URL = st, 1979
Store type = remote
Server url = http://sesame:8080/openrdf-sesame
repository = whichever one you created on http://localhost:10150/openrdf-workbench
username = null
password = null
```

