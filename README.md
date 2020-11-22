# Docker

```
$ docker build -t user_name/nginx-demo:v1 --no-cache .
$ docker run -it -p 3003:80 user_name/nginx-demo:v1
```

```
$ curl http://localhost:3003/hello/

<!DOCTYPE html>
<html>
	<header><title>Docker demo</title></header>
	<body style="text-align: center; margin-top: 10%">
	<h1>Hello from nginx running on Docker</h1>
	 <img style="margin-top: 5%" src="https://pluralsight2.imgix.net/paths/images/docker-copy-3135ce60d0.png" alt="Docker in ecs" >
	</body>
</html>
```

## Docker Hub Authentication

```
$ docker login

Login with your Docker ID to push and pull images from Docker Hub. If you don't have a Docker ID, head over to https://hub.docker.com to create one.
Username: user_name
Password:
```

```
$ docker push user_name/nginx-demo:v1
```