### node-docker

This is a simple example of running the node server on docker container.

0. run `eval $(docker-machine env)`
1. run `docker build -t <your-username>/node-docker .` 
2. run `docker run -i -t -p 2346:8080 <your-username>/node-docker` (you can also add `-d` to run it in the background)
3. run `docker-machine ls` and obtain a "real" URL, eg. `192.168.99.100`
4. run `curl -i <real-address-from-above>:2346`. Voila! 

