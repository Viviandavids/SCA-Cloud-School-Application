# SCA-Cloud-School-Application

Dear SCA,

I trust you find this well

Kindly find my first assessment for the SCA Cloud School Application.

https://hub.docker.com/repository/docker/vivian1807/sca_viviandavids


SHECODE APP

Using docker container to output webpage app

PREREQUISITES
git
docker

N.B docker should be installed and running on any system used

SETUP
The app can be setup either by pulling the docker image directly from docker hub or cloning the repository from github.

PULLING IMAGE FROM DOCKERHUB
1. Go to dockerhub to check for the shecode app image using this link:

https://hub.docker.com/repository/docker/vivian1807/sca_viviandavids


2. Next, pull the image into your machine or system using the command 

docker pull <imagename>:tagname

example:

docker pull vivian1807/sca_viviandavids:v2


3. Start the docker container using the command

docker run -it -d -p 8080:80 <imagename>


4. Next, access the application webpage using any browser on 

localhost:8080 or IP_ADDRESS:8080 (if you are using a machine)



CLONING REPOSITORY FROM GITHUB
1. Clone the application repository

git clone https://github.com/Viviandavids/SCA-Cloud-School-Application.git


2. Switch to the branch Start or branch feature using:

git checkout <name of branch>

example:
git checkout Start


3. Navigate into the docker folder containing the Dockerfile and then build the docker image using the command:

docker build -t <preferred name of image>:tag . 

example:

docker build -t vivian:v1 .

N.B -  The dot at the end of the command signifies the current directory


4. Start the container using the comand:

docker run -it -d -p 8080:80 <imagename>


5. Access the application webpage using any browser on 

localhost:8080 or IP_ADDRESS:8080 (if you are using a machine)



TESTING THE APPLICATION

1. Run the command:

docker ps 

N.B After running the command, under the status column, you should see running and also the port number

2. Open your browser and enter:

localhost:8080 to see the application
