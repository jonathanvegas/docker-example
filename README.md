# Docker Example

## to build an image
docker build -t 'bocacode':1.0 .

## to create a container
docker run --rm -d -p 8000:8000/tcp bocacode:1.0

## another line
docker run --rm -d -p 8000:8000/tcp -v $HOME/bocacode/docker-example:/src/ bocacode:1.0