<div align="center">
  <img src="/docs/docs/assets/img/lilbox.svg" height="200"/>
</div>

<h1 align="center" style="margin-top: -10px"> HomeBox </h1>
<p align="center" style="width: 100;">
   <a href="https://hay-kot.github.io/homebox/">文档</a>
   |
   <a href="https://homebox.fly.dev">演示</a>
</p>

## 快速开始

[配置 ducker run启动](https://hay-kot.github.io/homebox/quick-start)

```bash
# If using the rootless image, ensure data 
# folder has correct permissions
mkdir -p /path/to/data/folder
chown 65532:65532 -R /path/to/data/folder
docker run -d \
  --name homebox \
  --restart unless-stopped \
  --publish 3100:7745 \
  --env TZ=Europe/Bucharest \
  --volume /path/to/data/folder/:/data \
  ghcr.io/hay-kot/homebox:latest
# ghcr.io/hay-kot/homebox:latest-rootless
```

<!-- CONTRIBUTING -->
## 贡献

本项目来源[原作者](https://github.com/hay-kot/homebox)

贡献使开源社区成为一个学习、启发和创造的神奇场所。你所做的任何贡献我们都非常感激。

如果你不是程序员，你仍然可以在经济上做出贡献。财务捐助帮助我优先处理这个项目，并帮助我了解项目开发的实际需求。

<a href="https://www.buymeacoffee.com/haykot" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-green.png" alt="Buy Me A Coffee" style="height: 30px !important;width: 107px !important;" ></a>
## Credits

- Logo by [@lakotelman](https://github.com/lakotelman)
