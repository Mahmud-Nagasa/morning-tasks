# Docker

1. What is containerization, and how does it differ from virtualization?

#answer 
Containerization is a lightweight form of virtualization that allows us to package an application and its dependencies together into a single unit called a container. 

2. Why is containerization important in modern software development and deployment?

# answer 

important in modern software development and deployment because it offers a standardized and efficient way to package, distribute, and run applications.


3. What is the difference between an image and a container in Docker?
 # answer 

 Images are read-only templates containing instructions for creating a container. A Docker image creates containers to run on the Docker platform. while a container is an isolated place where an application runs without affecting the rest of the system and without the system impacting the application.


4. Can you give an example of a situation where you might choose to use Docker containers in a software development project?

# answer 
it has many uses one of them is Service Isolation, in service isolation each microservice can be packaged into its own Docker container. This container encapsulates the service's code, dependencies, and configuration. Isolating services in containers helps ensure that changes or updates to one service do not affect others.

5.If you were tasked with explaining Docker to someone who has never heard of it before, how would you describe it in a few sentences?

# answer 

I would say it's kind of like a usb stick that have a game installed inside of it, you can play the game once you have plugged the usb stick you don't need to go with installation process just connect and play 

## Extension

Fill in this cheat sheet throughout the day to help and remind you understand how to use Docker commands

| Command | Description |
| :-----: | ----------- |
|   ps    |
| images  |
|  pull   |
|  build  |
|   run   |
|  stop   |

| Flag | Description  
|:------:|---------------------------------------------------
| -a |
| -d |
| -t |
| -p |

Below is an example of a how you might format a docker command. (In documentation having something wrapped in square brackets [] denotes that it is optional to provide this in the command)

```bash
docker run [OPTIONS] <IMAGE[:TAG|@DIGEST]> [COMMAND] [ARG...]
```
