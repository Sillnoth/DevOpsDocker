FROM alpine:latest

RUN apk add mono --update-cache --repository http://nl.alpinelinux.org/alpine/edge/testing/ --allow-untrusted && rm -Rfv /var/cache/apk/*

COPY server.exe /usr/src/app/

EXPOSE 9090

CMD ["mono", "/usr/src/app/server.exe"] 
