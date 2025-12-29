FROM debian:bookworm-slim
		
RUN mkdir -p /var/www/html/
COPY ./index.html /var/www/html/
COPY ./tiny /
COPY ./flag /

RUN chmod 700 /tiny

CMD ["/tiny", "/var/www/html", "8000"]
