FROM lsioarmhf/nginx-armhf:115

MAINTAINER Wenpeng Xiao <xiaowp@flamingoeda.com>

# Copy assets
COPY ./nginx/site-confs /config/nginx/site-confs
COPY ./nginx/codeplayerbox-cert/certs/codeplayerbox-server.crt /config/keys/codeplayerbox-server.crt
COPY ./nginx/codeplayerbox-cert/certs/codeplayerbox-server.key /config/keys/codeplayerbox-server.key
