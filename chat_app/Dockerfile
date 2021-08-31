#go version
FROM golang:1.16.3-alpine
# update
RUN apk add --update && apk add git
# make directory
RUN mkdir /go/src/app
# set workdir
WORKDIR /go/src/app
# add files to container
ADD . /go/src/app
# ADD app/go.mod .
# ADD app/go.sum .

# download packages
RUN go mod download

EXPOSE 9000