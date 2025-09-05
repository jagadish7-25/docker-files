FROM almalinux:9
LABEL maintainer="jag"
LABEL email="jag@gmail.com"
RUN dnf -y install nginx && \
    rm -f /usr/share/nginx/html/index.html

COPY index.html /usr/share/nginx/html/index.html

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]
