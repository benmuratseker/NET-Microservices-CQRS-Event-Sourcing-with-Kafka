# NET Microservices CQRS & Event Sourcing with Kafka
###Set up Environment
- Docker network create --attachable -d bridge mydockernetwork
- Docker-compose up -d (on yml file location)
- Docker run -it -d --name mongo-container -p 27017:27017 --network mydockernetwork --restart always -v mongodb_data_container:/data/db mongo:latest
- docker run -d --name sql-container --network mydockernetwork --restart always -e "ACCEPT_EULA=Y" -e "SA_PASSWORD=$tr0ngP@ssw0rd01" -e 'MSSQL_PID=Express' -p 1433:1433 mcr.microsoft.com/mssql/server:2017-latest-ubuntu![image](https://github.com/benmuratseker/NET-Microservices-CQRS-Event-Sourcing-with-Kafka/assets/8171384/b7839263-1dbf-4d60-aa5b-c8fa06c13f15)
