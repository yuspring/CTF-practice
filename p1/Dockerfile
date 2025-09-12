FROM alpine:3.22
RUN apk update && apk add socat

COPY ./chal /
COPY ./flag /

CMD ["socat", "TCP-LISTEN:8000,fork", "EXEC:/chal"]