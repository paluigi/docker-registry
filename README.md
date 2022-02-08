# Registry with UI

Creates a local Docker registry bound to port 5001 on localhost  
No authentication  
GUI by joxit  

Usage:  
`docker-compose -f simple.yml up -d`

After that, if you want to create your local Python 3.9.10 image:  
`docker pull python:3.9.10-slim-buster
docker tag python:3.9.10-slim-buster localhost:5001/python:3.9.10-slim-buster
docker push localhost:5001/python:3.9.10-slim-buster`


References:
- Joxit examples [link](https://github.com/Joxit/docker-registry-ui/tree/main/examples/ui-as-standalone)
- Docker Registry documentation [link](https://docs.docker.com/registry/)

Soon to be published as tutorial at RandomDS [blog](https://randomds.com/blog/)
