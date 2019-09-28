# Docker-MusicBot

Dockerfile for [jagrosh/MusicBot](https://github.com/jagrosh/MusicBot)

## How to run
1. Create a `config` folder and create a `config.txt` file based on `config.txt.example` in there.
2. Edit the config as you'd like (token and owner are required fields)
3. Run the docker image
```
docker run -d --name musicbot -v $(pwd)/config:/usr/src/musicbot/config liljebergxyz/musicbot:latest
```
Or build and run it yourself
```
docker build . -t musicbot
docker run -d --name musicbot -v $(pwd)/config:/usr/src/musicbot/config musicbot
```
