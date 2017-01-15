# Introduction to Golang Docker

You could simply create an alias to make use of Golang docker image.

```sh
alias go="docker run -it -v $GOPATH:/go --rm golang:1.7.4-alpine go"
```

With the alias we can now install packages like this:

```sh
go install $GOPATH/src/github.com/shavenking/hello
```

P.S. You should export `$GOPATH/bin` to your `$PATH`.