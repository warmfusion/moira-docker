FROM golang:1.7

# http://moira.readthedocs.org/en/latest/quickstart.html


# Install the libraries we need
ENV GOPATH /moira
RUN go get github.com/moira-alert/cache
RUN go get github.com/moira-alert/notifier/notifier

RUN mkdir /var/log/moira/
