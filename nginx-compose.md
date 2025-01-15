---
version: '3.8'
services:
 tomcat:
  image: tomee
  container_name: tomcat_server
  ports:
   - "8087:8080"
 nginx:
  image: nginx:latest
  container_name: nginx_server
  ports:
   - "85:80"

nginx-tomcat