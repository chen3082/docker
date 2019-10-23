# docker
in ubuntu16.04

Install docker first

Following this link

https://www.vultr.com/docs/installing-docker-ce-on-ubuntu-16-04

To build the image: sudo docker build -t first .

To run the image: sudo docker run --net=host -it -e DISPLAY=$DISPLAY first
