# FSoft_DevOps_Course
Name: Canh Nguyen
Account: CanhND2
Business Unit: FHN.BU9

Build image:
```
docker build -t root_war:1.0 . or docker build -t root_war .
```

Run image:
```
docker run -p 8080:8080 root_war:1.0 or docker run -p 8080:8080 root_war
```

Create network:
```
docker network create --subnet 10.10.20.0/24 --driver bridge DevOps_Bridge_Network
```

Run image on DevOps_Bridge_Network:
```
docker run -p 8080:8080 -d -it --network=DevOps_Bridge_Network --name=devops root_war
```

Link Job:
https://jenkins.learn.akawork.io/job/CanhND2/job/Pipeline-for-final-test 
