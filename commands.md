pip freeze
# describe what this does
pip freeze > requirements.txt


docker build --pull -t <tag_name> .
docker run -p 8080:8080 -v <your_local_repo>:<path_in_container> -it <tag_name>

### show all the running docker processes
docker ps

docker stop <container_id>


