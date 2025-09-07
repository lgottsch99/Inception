FROM debian:12

#RUN runs wehen building img
#download + configure nginx
RUN apt update
RUN apt install nginx -y

RUN apt install ufw -y
#RUN  ufw enable
RUN ufw allow 443


#runs when running cont
CMD ["ufw status"]