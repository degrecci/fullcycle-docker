# FROM nginx:latest

# WORKDIR /app
# RUN apt-get update && \
#     apt-get install vim -y

# COPY html/ /usr/share/nginx/html

# Delete all containers running 
# docker rm $(docker ps -a -q) -f


# ENTRYPOINTs e CMD
# FROM ubuntu:latest

# ENTRYPOINT [ "echo", "Hello " ]
# CMD ["World"]

FROM nginx:latest

COPY html /usr/share/nginx/html

ENTRYPOINT ["/docker-entrypoint.sh"]
CMD ["nginx", "-g", "daemon off;"]

# Access internal from docker container, http://host.docker.internal:8000