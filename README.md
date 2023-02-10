&nbsp;

<div align="center">
  <img src="./assets/clash.png" width="35%" alt="clash" />
  <p>
    <b>A rule-based tunnel in Go. Forked from <a href="https://hub.docker.com/r/xtoys/clash">xtoys/clash </a>. </p>
    <b>Modified for me only, but may work for you.</b></p>
    <b> More platforms supported: linux/amd64, linux/arm64, linux/arm/v8(aarch64), linux/arm/v7</b></p>
    linux/armv6 is to be continued </p>
    <b>Thanks to <a href="https://github.com/uxber">uxber</a> and <a href="https://github.com/Dreamacro">Dreamacro</a> </b>
  </p>
  <p>
    <a href="https://github.com/uxber/clash/wiki">WIKI</a> · <a href="https://github.com/Dreamacro/clash/releases/tag/premium">CHANGELOG</a>
  </p>
</div>

# Usage
```
docker run -d \
 --name clash-dev \
 -p 901:901 \
 -p 7890:7890 \
 --hostname clash \
 --restart unless-stopped \
 -v /storage/clash/config:/clash/config \
 bohong65/clash-docker:latest
 ```
 
TIPS: Make sure to add following config into your `config.yaml`
```
mixed-port: 7890
allow-lan: true
external-controller: 127.0.0.1:901
```
Yacd web panel: `host-ip:9090/ui`

