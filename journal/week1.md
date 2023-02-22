# Week 1 — App Containerization

## Tasks achieved

For this weeks challenge, it was all about containerization of the cruddur apps, i. the frontend and backend applications.

The created dockerfiles for the backend and frontend applications, reside in their respective folder, with the docker compose file inside the main folder housing the application folders.

The created frontend image can be found in my docker hub repo which can be accessed [here](https://hub.docker.com/r/achebeh/aws-cruddur-2023-webapp) and the backend  image [here](https://hub.docker.com/r/achebeh/aws-cruddur-2023-flaskapp)

![](/Week1_Documents/1.png)

To pull the image from the CLI
```
docker pull achebeh/aws-bootcamp-cruddur-2023-flaskapp
```
```
docker pull achebeh/aws-bootcamp-cruddur-2023-webapp
```

A sample image of the app running from the conatiner is shown below.

![](/Week1_Documents/2.png)

Health check for the Flask app was also implemented, this check was to ensure the flaskapp was up and running. The health check implemented is found below.
```
    healthcheck:
      test: curl --fail https://4567-${GITPOD_WORKSPACE_ID}.${GITPOD_WORKSPACE_CLUSTER_HOST} || exit 1
      interval: 30s
      timeout: 30s
      retries: 3
      start_period: 0s

```

To demonstrate the created images running in a local environment outside the gitpod enironment I installed docker on my Ubuntu environment using the instruction laid [here](https://docs.docker.com/engine/install/ubuntu/) . 

![](/Week1_Documents/3.png)

The following images are screenshots of the frontend and backend apps working in my local ubuntu environment.

![](/Week1_Documents/4.png)

![](/Week1_Documents/5.png)

Lastly, to demonstrate the created images can be used anywhere, I was able to pull and run the image from a created AWS EC2 instance.

Below is a screenshot of the imagee being pulled and run from the AWS CLI, the running application can also be accessed [here](http://54.160.155.76:3000/)

![](/Week1_Documents/6.png)


