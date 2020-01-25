### Tags

4.39, 4.39-amd64, amd64, latest

[![](https://images.microbadger.com/badges/image/kgotso/kodexplorer.svg)](https://microbadger.com/images/kgotso/kodexplorer "Get your own image badge on microbadger.com")

4.39-arm, arm 

[![](https://images.microbadger.com/badges/image/kgotso/kodexplorer:arm.svg)](https://microbadger.com/images/yangxuan8282/kodexplorer:arm "Get your own image badge on microbadger.com")

### RUN

```
docker run -d -p 80:80 --name kodexplorer -v "$PWD":/var/www/html kgotso/kodexplorer
```


### Dockerfile

https://github.com/kgotso/docker-image/tree/master/kodexplorer

### Docker Compose

```
version: "2"

services:
  kodexplorer:
    image: kgotso/kodexplorer
    restart: "always"
    ports:
      - "80:80"
    volumes:
      - "./html:/var/www/html"
```
