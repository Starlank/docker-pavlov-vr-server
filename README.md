# docker-pavlov-vr-server

Docker container which runs a PavlovVR Server


Build & Tag:
```
docker build -t pavlov:1.0 .
```

Run with default settings (none of the ports will be forwarded):
```
docker run -it --user steam pavlov:1.0
```

Run opening default ports
```
docker run -it --user steam -p 7000:7000 -p 7200:7200 -p 7777:7777 pavlov:1.0
```

Run using docker-compose, which has configuration to manage the settings:
```
docker-compose up
```
