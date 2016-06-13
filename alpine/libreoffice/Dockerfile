FROM alpine:latest
MAINTAINER xfsuper@gmail.com

RUN apk update && apk add libreoffice

EXPOSE 8997

# replace default setup with a one disabling logos by default
ADD sofficerc /etc/sofficerc
ADD startoo.sh /usr/bin/startoo.sh

VOLUME ["/tmp"]

RUN chmod +x /usr/bin/startoo.sh

ENTRYPOINT ["/usr/bin/startoo.sh"]
