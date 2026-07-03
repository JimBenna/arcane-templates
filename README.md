This repo stores examples of docker-compose.yml ready to use.

to create specific user system account on debian use
```shell
useradd -c "User Description" -N -G docker -g 65534 -d /nonexistent -r -s /usr/sbin/nologin -M <username>
```
