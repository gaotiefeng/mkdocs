## MkDocs in Docker
[![build status badge](https://travis-ci.org/youmingdot/docker-mkdocs.svg)](https://travis-ci.org/youmingdot/docker-mkdocs)
[![layers badge](https://images.microbadger.com/badges/image/youmingdot/mkdocs.svg)](https://microbadger.com/images/youmingdot/mkdocs)
### Supported tags and respective Dockerfile links

+  `0.15.3`, `0.15`, `latest` [(cron/Dockerfile)](https://github.com/youmingdot/docker-mkdocs/blob/master/0.15/Dockerfile)

------
### Author
+ You Ming (youming@funcuter.org)

------
### Usage

##### Run as a development server
```
$ docker run -d --name mkdocs -v /path/to/src:/docs/src youmingdot/mkdocs:latest -s
```

##### Build the MkDocs documentation
```
$ docker run -t --name mkdocs --rm -v /path/to/src:/docs/src -v /path/to/output:/docs/output youmingdot/mkdocs:latest -b
```

##### Or build to JSON files
```
$ docker run -t --name mkdocs --rm -v /path/to/src:/docs/src -v /path/to/output:/docs/output youmingdot/mkdocs:latest -j
```
