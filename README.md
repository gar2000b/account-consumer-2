# account-consumer-2
Account Consumer 2

docker network create -d bridge account 
docker network ls  

docker build -t gar2000b/account-consumer-2 .  
docker run -it -d -p 9087:9087 --network="account-consumer-2" --name account-consumer-2 gar2000b/account-consumer-2  

All optional:

docker create -it gar2000b/account-consumer-2 bash  
docker ps -a  
docker start ####  
docker ps  
docker attach ####  
docker remove ####  
docker image rm gar2000b/account-consumer-2  
docker exec -it account-consumer-2 sh  
docker login  
docker push gar2000b/account-consumer-2  