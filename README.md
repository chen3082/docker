# Flappy

Flappy Hummingbird: An Open Source Dynamic Simulation of Flapping Wing Robots and Animals

This still work in progress. Full version will be released by May 20th 2019 and presented at ICRA2019.

![](demo.gif)

## Publication

To cite this work in publications:

	@inproceedings{fei2019flappy,
	  title={Flappy Hummingbird: An Open Source Dynamic Simulation of Flapping Wing Robots and Animals},
	  author={Fei, Fan and Tu, Zhan and Yang, Yilun and Zhang, Jian and Deng, Xinyan},
	  booktitle={2019 IEEE International Conference on Robotics and Automation (ICRA)},
	  year={2019},
	  organization={IEEE}
	}

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Alternative installation methods
1. Pydart2 source code included in our project. (No extra installation required) 
	[No installation](https://github.com/chen3082/flappy)
2. Pydart2 source code not included in our project. (Installation required, which is not a pleasant experience.) 
	[Installation required](https://github.com/purdue-biorobotics/flappy)
3. Docker (If you do not have access to recommanded OS environment) 
	* Please continue your steps here
  
### Prerequisites
If you do not use Ubuntu 16.04, please consider using our docker file. Everything needed for this project is wrapped in the docker file. You can either compile the docker file in this repository or the use docker image we have compiled directly.


## Docker container
# In ubuntu16.04

* First install docker  
  Following this [Document](https://www.vultr.com/docs/installing-docker-ce-on-ubuntu-16-04)

* Clone the repository:
  ```zsh
  git clone https://github.com/chen3082/docker.git
  ```
* Build the image: 
  ```zsh
  sudo docker build -t first .  
  ```
* Run the image: 
  ```zsh
  sudo docker run --net=host -it -e DISPLAY=$DISPLAY first
  ```

## Environment and testing
* To change the command you are running, please modify the command in the docker file
  ```zsh
  CMD ["python3", "test.py", "--model_type=PID"]
  ```
 * If you are using one of our image file and want to have different command, you can request that and we will compile the new docker file for you
