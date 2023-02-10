&nbsp;

<div align="center">
  <img src="./assets/clash.png" width="35%" alt="clash" />
  <p>
    <b>A rule-based tunnel in Go. Forked from [xtoys/clash](https://hub.docker.com/r/xtoys/clash). Modified for me only, but may work for you.</b></p>
   <b> More platforms supported: linux/amd64,linux/arm64,linux/arm/v8(aarch64),linux/arm/v7</b></p>
    linux/armv6 is to be continued </p>
    <b>Thanks to <a href="https://github.com/uxber">uxber</a> and <a href="https://github.com/Dreamacro">Dreamacro</a> </b>
  </p>
  <p>
    <a href="https://github.com/uxber/clash/wiki">USAGE</a> · <a href="https://github.com/Dreamacro/clash/releases/tag/premium">CHANGELOG</a>
  </p>
</div>
---
# Usage
```
docker run -d \
 --name clash \
 --network host \
 --hostname clash \
 --restart unless-stopped \
 bohong65/clash-docker:latest
 ```
 
You can choose to mount `/clash` folder to anywhere you like on your host, but mounting using `docker run -v` command is NOT recommended cause Yacd directory`/clash/ui` will not be created. This is a bug in [xtoys/clash](https://hub.docker.com/r/xtoys/clash), may be fixed here in future release.

Yacd web port: `ip:9090/ui`

&nbsp;
