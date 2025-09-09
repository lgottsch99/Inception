FROM debian:12

#RUN runs wehen building img
#download + configure nginx
RUN apt update -y
RUN apt install nginx -y

COPY default /etc/nginx/sites-available/.
#RUN apt install ufw -y  ->containers dont control HOST FIREWALL lol
#RUN  ufw enable
#RUN ufw allow 443


#runs when running cont
#CMD ["echo", "hi hellooo"]
#CMD -> becomes pid1!!! The container lives and dies with PID 1. If PID 1 exits, the container exits.
# -g overrides anything specified in config file
CMD ["nginx", "-g", "daemon off;"]
# CMD ["cat", "/etc/nginx/nginx.conf"]

#configure nginx using config file?
