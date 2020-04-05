# Install Grafana locally from the Docker image

This guide will help you to install Grafana locally from the Docker image, open it in a browser on a localhost. Also, it will show you how to create a test dashboard from the TestDataDB source.


## Getting Started

Firstly, to get Grafana installed from Docker you need to decide which image of Grafana to choose: either * [Alpine](https://hub.docker.com/_/alpine) or [Ubuntu](https://hub.docker.com/_/ubuntu).  Alpine one is smaller and more secure because it’s base distribution is [Alpine Linux](https://alpinelinux.org/), that is small by its nature. Ubuntu-based image is for those, who prefer [Ubuntu](Ubuntu) and/or who are dependent on certain tooling not available for Alpine.

Secondly, you need to go to the Docker image, choose architecture, look for tag ubuntu: latest, that will ensure the latest version of the image and copy-paste command in your terminal. After that image will be installed:
![](https://github.com/vladshu20/tech-writer/blob/pictures/image5.png)


To test installation try to execute the next command, which will run Grafana: 
```
docker run -d -p 3000:3000 grafana/grafana.
```

### Note: If you are on a Linux system, you might need to add sudo before the command.

### Prerequisites

you need to get Docker installed


### Running grafana locally in your browser

After that please go to localhost:3000 in your browser. You are about to see a screen with authentification.
![](https://github.com/vladshu20/tech-writer/blob/pictures/image2.png)

Enter user/password as admin/admin. PLEASE, do not forget to change the password later.

### How to create a test dashboard from the TestDataDB source.

After you’ve entered  you’ll see  banner:
![](https://github.com/vladshu20/tech-writer/blob/pictures/image1.png)


For this example, I’ve already created a data source and built a dashboard, that’s why these points are crossed. You’ll have to click on these points to add a data source and here is what you are going to face:
![](https://github.com/vladshu20/tech-writer/blob/pictures/image4.png)

If you scroll down, you’ll see :
![](https://github.com/vladshu20/tech-writer/blob/pictures/image6.png)

 After that, please click select. On the next page, click save & test. On the left panel you’ll see “plus” sign. Click on it and choose the “dashboard” option.
 ![](https://github.com/vladshu20/tech-writer/blob/pictures/image3.png)


In settings of the new dashboard in query option choose name of your data source.









## Official documentation

Please read [Grafana documentation](https://grafana.com/docs/grafana/latest/) for details.


