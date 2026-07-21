FROM almalinux:9

RUN dnf install nginx -y

RUN rm -rf /usr/share/nginx/html/index.html

ADD https://raw.githubusercontent.com/Pardhu-mutyala/DevOps-leaning/refs/heads/main/vmss.md /usr/share/nginx/html/index.html

RUN chmod +r /usr/share/nginx/html/index.html

CMD ["nginx", "-g", "daemon off;"]
