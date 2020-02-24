# How to do the demo

!!! MAKE SURE DOCKER IS RUNNING !!!

1. Open VSCode
2. Create a Dockerfile

```Dockerfile
FROM httpd:latest

COPY ./public-html/ /usr/local/apache2/htdocs/

EXPOSE 80
```

3. Run locally

`cd demo-site`

`docker build --tag 'dotnetnotts' . `

`docker run -d -p 80:80 dotnetnotts`

4. Create YAML build for Azure DevOps

5. Commit and push

6. Go to Azure DevOps

7. Go to Docker Hub


Make a change to the site content. Add this gif: https://media.giphy.com/media/WrgtbRE1zywNy/giphy.gif

# Useful commands

Stop runnining containers:

`docker stop $(docker ps -a -q)`

Remove images:

`docker rm $(docker ps -a -q)`