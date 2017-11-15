## Pane 1
`docker build -t USERNAME/REPO:TAG .`
build container

`docker run -e DISPLAY=$(ifconfig en0 | grep 'inet ' | cut -d" " -f2):0 --name xeyes x11:latest`
- run command in a new container
- -e designates entrypoint
`DISPLAY` is set by bash expansion
--name give unique name to container



## Pane 2
`socat TCP-LISTEN:6000,reuseaddr,fork UNIX-CLIENT:\"$DISPLAY\"`
