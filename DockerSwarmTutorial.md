## At Leader:

      docker swarm init

      docker node ls
      docker service create -p 80:80 --name web nginx:latest
      docker service ls

      curl http://localhost:80
      docker node ls
      docker ps
      docker service inspect web
      docker service scale web=15
      docker service ps web
      docker node update --availability drain node2
      docker service ps web
      docker ps
      docker ps|wc -l
      docker service scale web=15
      docker ps|wc -l
      docker service scale web=10
      docker ps|wc -l
      docker service ps web
      docker node update --availability active node2
      docker service ps web
      docker node ls
      docker node inspect node2 --pretty

## AT worker node2

      docker swarm join --token SWMTKN-1-3jqt6ertjmu2to60vu0ddraelkpne9shzth3igefxk85iow7b0-4cscwbsrtskgpalsumcivpl8u 192.168.0.18:2377
      docker ps -a
      docker node ls
      curl http://localhost:80
      docker ps

   
   
