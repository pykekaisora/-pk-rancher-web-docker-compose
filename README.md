# PK Rancher Server Docker Compose

Just found 2 ways to do rancher:
1. Use Host Network
2. containerized it

## Rancher Server Web Default Network
I've added a network and called it `rancher-connector` so if you spun up postgresql or mysql, remember to attached `rancher-connector` to phpmyadmin or adminer to their container

## Rancher Server Host Network
You'll use the host's networks and ports directly as if you are installing it on your OS except the part you'll still need to use `$ docker exec -it rancher-web bash` to use Kubernetes, containerd and etc.