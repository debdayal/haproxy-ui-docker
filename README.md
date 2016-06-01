# UI Load balancer with haproxy
Use git clone https://github.com/debdayal/haproxy-ui-docker.git
> cd haproxy-ui-docker

Adjust the **haproxy.conf** based on the environment.

In this case it is assumed that two nginx webservers are running at below address.

*192.168.33.10:8001*

*192.168.33.10:8002*

> docker build --force-rm -t **your_name**/haproxy-ui .

> docker run -d -p 80:80 --name haproxy-ui -t **your_name**/haproxy-ui

You may want to push to DockerHub with below command

> docker login

> docker push **your_name**/haproxy-ui
