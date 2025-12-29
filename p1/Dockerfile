FROM debian:trixie-slim
RUN apt-get update && apt-get install -y socat && rm -rf /var/lib/apt/lists/*

COPY ./chal /
COPY ./flag /

RUN chmod 700 /chal 

CMD ["socat", "TCP-LISTEN:8000,fork", "EXEC:/chal"]