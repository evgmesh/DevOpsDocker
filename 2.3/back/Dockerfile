FROM ubuntu

COPY . .

RUN apt-get update && apt-get install -y wget gcc 
RUN wget -c https://golang.org/dl/go1.16.4.linux-amd64.tar.gz 

RUN rm -rf /usr/local/go && tar -C /usr/local -xzf go1.16.4.linux-amd64.tar.gz

ENV REQUEST_ORIGIN http://localhost:5000

ENV PATH=$PATH:/usr/local/go/bin

RUN go build 

RUN go test 

EXPOSE 8080

CMD ["./server"]

