### Docker-mongodb


### Usage

#### Build

```
git clone https://github.com/stumpyfr/docker-mongodb.git
cd docker-mongodb
docker build -t stumpy/mongodb:2.6.2 .
```

#### Run `mongod`

`docker run -d -p 27017:27017 --name mongodb stumpy/mongodb:2.6.2`

#### Run `mongod` with mounted volume

`docker run -d -p 27017:27017 -v <data-dir>/db:/data/db --name mongodb stumpy/mongodb:2.6.2`