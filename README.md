![Docker Pulls](https://img.shields.io/docker/pulls/muenchdo/hello-name)
# Hello Name

This is a simple Docker image which extends the awesome [docker-hello-world](https://github.com/crccheck/docker-hello-world) by allowing you to configure who to greet on the index page.

## Sample Usage

### Starting a web server on port 8000

```bash
$ docker run -d --rm --name hello -p 8000:8000 -e NAME=Stranger muenchdo/hello-name
```

The server will now greet you with the name you set via the environment variable `NAME`:

```
$ curl localhost
<xmp>
Hello Stranger


                                       ##         .
                                 ## ## ##        ==
                              ## ## ## ## ##    ===
                           /""""""""""""""""\___/ ===
                      ~~~ {~~ ~~~~ ~~~ ~~~~ ~~ ~ /  ===- ~~~
                           \______ o          _,/
                            \      \       _,'
                             `'--.._\..--''
</xmp>
```
