FROM nginx:1.19.8

#RUN groupadd --gid 2000 docker_group \ 
#    && useradd --uid 2000 --gid docker_group -m docker_user \ 
#    && chown -R docker_user:docker_group /var \ 
#    && chown -R docker_user:docker_group /run 
 
#USER docker_user 

COPY html/ /var/www/html
COPY default.conf /etc/nginx/conf.d/default.conf
COPY nginx.conf /etc/nginx/nginx.conf
#COPY cert/ /etc/letsencrypt/live/task14.ddnsking.com


#EXPOSE 80 443

#CMD ["/usr/sbin/nginx", "-g", "daemon off;"]
