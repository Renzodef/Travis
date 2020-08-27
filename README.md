## PREREQUISITES
- Register at: https://hub.docker.com/
- Register at: https://github.com/
- Connect Github with Travis by signing in at: https://travis-ci.org/
- Publish the Github repository

## TRIGGER THE BUILD
- Go in Travis website in the section settings and enable your new Github repository
- Go in the Travis dashboard and trigger the build
- Check into the Docker Hub website if the repository is added in the section Repositories.

## RUN THE CONTAINER
- Install Docker on your pc
- Get the image from terminal with: <br> 
docker pull <dockeruser/nameofproject> <br>
(Replace  <dockeruser/nameofproject> with the name of your Docker Hub repository)
- Run the container from terminal with: <br>
docker run --rm -d  -p 4000:4000/tcp <dockeruser/nameofproject>

## UPDATE THE REPOSITORY
- Just publish your changes into Github and all will be handled by Travis CI.