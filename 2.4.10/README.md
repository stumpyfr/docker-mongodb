### Docker-mongodb


### Usage

#### Build

```
git clone https://github.com/stumpyfr/docker-mongodb.git
cd docker-mongodb/2.4.10
docker build -t stumpy/mongodb:2.4.10 .
```

#### Run `mongod`

`docker run -d -p 27017:27017 --name mongodb stumpy/mongodb:2.4.10`

#### Run `mongod` with mounted volume

`docker run -d -p 27017:27017 -v <data-dir>/db:/data/db --name mongodb stumpy/mongodb:2.4.10`