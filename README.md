# docker
in ubuntu16.04

Install docker first

Following this link

https://www.vultr.com/docs/installing-docker-ce-on-ubuntu-16-04

To clone the repository:

git clone https://github.com/chen3082/docker.git

To build the image: 

sudo docker build -t first .  

To run the image: 

sudo docker run --net=host -it -e DISPLAY=$DISPLAY first
