FROM alpine:3.13

WORKDIR /usr/src/app

COPY hello.sh .

ENV REACT_APP_BACKEND_URL=http://localhost:8080

RUN touch additional.txt

CMD ./hello.sh
