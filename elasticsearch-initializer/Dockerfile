FROM bashell/alpine-bash:default

WORKDIR /tmp
COPY ./set_log_stash_index /tmp
COPY ls-es-template-20150831.json /tmp
RUN chmod +x ./set_log_stash_index

RUN apk add --update curl && rm -rf /var/cache/apk/*

CMD ./set_log_stash_index

