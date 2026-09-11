FROM almalinux:9
RUN dnf install nginx -y
## removing default index.html page
RUN rm -rf /usr/share/nginx/html/index.html
## ADD is taking details from internet and it will load into index.html
ADD https://raw.githubusercontent.com/daws-84s/notes/refs/heads/main/session-51.txt /usr/share/nginx/html/index.html
RUN chmod +r /usr/share/nginx/html/index.html
## index.html file has read access to load the data
ADD sample-1.tar /tmp/
## ADD command will do untar the sample-1.tar and place it in tmp/
CMD ["nginx","-g","daemon off;"]