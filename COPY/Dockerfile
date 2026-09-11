FROM almalinux:9
RUN dnf install nginx -y
## removing default index.html page
RUN rm -rf /usr/share/nginx/html/index.html
COPY index.html /usr/share/nginx/html/index.html
### COPY qi/ /usr/share/nginx/html/ ## qi/ directory will be loaded to html/ 
## need to copy qi/ from git folder 
CMD ["nginx","-g","daemon off;"]