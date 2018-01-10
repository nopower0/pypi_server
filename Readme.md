A simple Pypi server that hosts all packages under a root folder.
Sample run command:
```shell
docker run --detach \
    --publish 80:80 \
    --volume /package/folder/on/host:/packages \
    --name="pypi-server" \
    --restart always \
    nopower0/pypi-server
```