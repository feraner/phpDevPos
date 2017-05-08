#base image on alpine
FROM %auth%/alpine%suffix%:latest

#maintainer
MAINTAINER %auth% %email%

RUN apk update && apk upgrade

#apk install 
RUN apk add memcached

#expose
EXPOSE 11211

#volume

#exec user
USER daemon

#exec command when start container
CMD ["memcached", "-m", "128"]
