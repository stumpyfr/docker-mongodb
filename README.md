### Docker-mongodb


### Usage

#### Build

```
git clone https://github.com/stumpyfr/docker-mongodb.git
cd docker-mongodb
docker build -t stumpy/mongodb .
```

if you need a specific version:

```
git clone https://github.com/stumpyfr/docker-mongodb.git
cd docker-mongodb/x.y.z
docker build -t stumpy/mongodb:x.y.z .
```

#### Run `mongod`

`docker run -d -p 27017:27017 --name mongodb stumpy/mongodb`

or for a specific version

`docker run -d -p 27017:27017 --name mongodb stumpy/mongodb:x.y.z`

#### Run `mongod` with mounted volume

`docker run -d -p 27017:27017 -v <data-dir>/db:/data/db --name mongodb stumpy/mongodb`

or for a specific version

`docker run -d -p 27017:27017 -v <data-dir>/db:/data/db --name mongodb stumpy/mongodb:x.y.z`