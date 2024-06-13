FROM nginx:latest

VOLUME [ "nginx.conf" ]

ENTRYPOINT ["/docker-entrypoint.sh"]
CMD ["nginx", "-g", "daemon off;"]
