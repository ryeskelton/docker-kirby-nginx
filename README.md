Hi Puppies...

For a new kirby site

### fork this repo :)

### rename to project name

### fire up "Docker Quickstart Terminial"

Check that docker is running by running 

```
docker ps
```

Output should be:

```
CONTAINER ID        IMAGE               COMMAND             CREATED             STATUS              PORTS               NAMES
```
### on your local machine login to https://hub.docker.com account

```
docker login
```

### clone your forked Github repo

```
git clone -r http://yourrepo projectname
```

### pull the docker repo

```
docker pull jodie/docker-kirby-nginx
```

### run it:
```
docker run -i -t -p 80:80 -v $PWD:/app jodie/docker-kirby-nginx
```

it should say in site.php: you can change to map to a differest directory

```
<?php
$kirby = kirby();
$kirby->urls->index = '/';
```

### list running docker containers:
for good measure run:

```
docker ps
```

and your 
