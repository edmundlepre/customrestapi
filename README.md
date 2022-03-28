# customrestapi





<br><br>
##### Creating the Docker Image
<p align="left">
  <img src="https://www.docker.com/sites/default/files/d8/2019-07/horizontal-logo-monochromatic-white.png" height="40" />
</p>
Create our docker image with the "Dockerfile" from our repository by:

```
docker build -t gcr.io/${USER_ID}/tasks:v1 .
```

List your Docker images to verify.
```
docker images
```
##### Pushing the Docker image to the Container Registry


#### Docker Container
<p align="left">
  <img src="https://www.docker.com/sites/default/files/d8/2019-07/horizontal-logo-monochromatic-white.png" height="75" />
</p>

1. Install [Docker](https://docs.docker.com/get-docker/) and verify your installation with ``` docker -v ```
2. Launch the terminal in the library_api folder or direct to this directory.
3. Build the docker image (be sure to include the ". " at the end and to define your username ``` whoami```)

```
docker build -t <your username>/tasks . 
```

4. Run your container:
```
docker run -it -p 5000:5000 <your username>/tasks 
```

This will map port 5000 to the host 5000 in our container. 

5. Access the backend from your browser via ``http://localhost:5000``

More info: [Dockerizing a Node.js web app](https://nodejs.org/en/docs/guides/nodejs-docker-webapp/) 

