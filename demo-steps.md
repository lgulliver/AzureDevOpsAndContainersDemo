# How to do the demo

1. Open VSCode
2. Create a Dockerfile


```Dockerfile
FROM httpd:latest

COPY ./public-html/ /usr/local/apache2/htdocs/

EXPOSE 80
```
