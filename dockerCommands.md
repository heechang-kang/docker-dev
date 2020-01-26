# basic

## docker commands 

|                       |     |
| --------------------- | --- |
| docker info           |     |
| docker version        |     |
| docker container list |     |
| docker pull <image>   |     |

|                                             |                                              |
| ------------------------------------------- | -------------------------------------------- |
| docker container run                        |                                              |
| docker run <img>:<version>                  | the container is only running                |
| docker run -d <image>                       | runs in the background                       |
| docker run -i <img>                         | interactive;'-it' means interactive terminal |
| docker run -p 80:5000 <img>               | it is mapping the port/ p: port              |
|                                             | 80: user port 5000: internal                 |
| docker attach <image or id>                 |                                              |
| docker run -v <locExternal>:<locIn> <image> |                                              |
|                                             |                                              |
| docker build <dest>                         | build -t <name> <dest>                       |
|                                             |                                              |
|                                             |                                              |
| docker inspect <name>                       | when see env, u can use docker run -e <name> |
| docker logs <name>                          |                                              |
| docker stop                                 |                                              |
|                                             |                                              |
| docker rm                                   |                                              |
|                                             |                                              |
|                                             |                                              |
|                                             |                                              |
| docker exec cat <file>                      | run a command in the container               |

| dockerfile command                         |             |
| ------------------------------------------ | ----------- |
| RUN                                        |             |
| FROM                                       |             |
| CMD command , CMD ["command", "parameter"] |             |
| ENTRYPOINT                                 | add command |

| docker networking                |                                        |
| -------------------------------- | -------------------------------------- |
| default networks                 | *bridge(gives internal IP), none, host |
| docker run Ubuntu --network=host | connect to external                    |
|                                  |                                        |
|                                  |                                        |

|docker storage||
- file system : stores in /var/lib/docker --> /aufs, /containers, /image, /volumes
- layered architecture : can use cache
  - image layers, container layer(read&write) 

docker has DNS server