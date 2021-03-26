## Python requirements gathering

See all the packages installed
```bash
pip freeze
```

Install packages 
```bash
pip install <package_name>
```

Record all the install python packages:
```bash
pip freeze > requirements.txt
```

## Usefull Docker commands

#### Running docker containers
Build a docker image and give the image the name <tag_name>
```bash
docker build --pull -t <tag_name> .
```

Run the container with a given tag name:
```bash
docker run -p 8080:8080 -t <tag_name>
```

Run the container interactively with a given tag name:
```bash
docker run -p 8080:8080 -it <tag_name>
```

Run the container interactively with a mounted volume:
```bash
docker run -p 8080:8080 -v <your_local_repo>:<path_in_container> -it <tag_name>
```

#### Maintaining containers
Check all the running containers:
```bash
docker ps
```

Stop a running container:
```bash
docker stop <container_id>
```
