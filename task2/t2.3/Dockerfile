FROM nginx:1.19.6

MAINTAINER Valerii Nikolskyi <pheanixs@gmail.com>

# Give ARG DEVOPS a dafault value = Pheanix
ARG DEVOPS=Pheanix

# Assign the $DEVOPS arg to the DEVOPS ENV so that it can be accessed
# by the subsequent RUN call within the container
ENV DEVOPS $DEVOPS

COPY ./html/index.html /usr/share/nginx/html
