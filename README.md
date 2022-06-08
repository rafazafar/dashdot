<!-- markdownlint-disable -->
<h1>
  <img src=".github/images/banner_muted.png" alt="dash. - a modern server dashboard">
</h1>

<div align="center">
  <a href="https://drone.mauz.io/MauriceNino/dashdot" target="_blank">
    <img src="https://drone.mauz.io/api/badges/MauriceNino/dashdot/status.svg">
  </a>
</div>

<br/>

<p align="center">
  <b>dash.</b> (or <b>dashdot</b>) is a modern server dashboard, running on the latest tech, designed with glassmorphism in mind. It is intended to be used for smaller VPS and private servers.
</p>
<br />
<p align="center">
  <a href="https://dash.mauz.io" target="_blank">Live Demo</a>
 |
  <a href="https://hub.docker.com/r/mauricenino/dashdot" target="_blank">Docker Image</a>
</p>

#

<a href="https://ko-fi.com/mauricenino" target="_blank">
  <img 
    align="right"
    width="160"
    style="padding-left: 20px; padding-bottom: 10px"
    alt="Consider sponsoring the development of this project"
    src="https://cdn.ko-fi.com/cdn/kofi2.png?v=3"
  />
</a>

<!-- markdownlint-enable -->

**dash.** is a open-source project, so any contribution is highly appreciated.
If you are interested in further developing this project, have a look at the
[Contributing.md](./CONTRIBUTING.md).

In case you want to financially support this project, you can visit my
[GitHub Sponsors](https://github.com/sponsors/MauriceNino), or my [Ko-Fi](https://ko-fi.com/mauricenino).

## Preview

<!-- markdownlint-disable -->

| Dark-Mode                                                                              | Light-Mode                                                                               |
| -------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- |
| <img src=".github/images/screenshot_darkmode.png" alt="Screenshot of the dark-mode" /> | <img src=".github/images/screenshot_lightmode.png" alt="Screenshot of the light-mode" /> |

<!-- markdownlint-enable -->

## Documentation

- [Installation Options](./INSTALL.md)
- [Configuration Options](./CONFIGURATION.md)
- [Contributing](./CONTRIBUTING.md)
- [Changelog](./CHANGELOG.md)

## Quick Install (Docker)

Images are hosted on [DockerHub](https://hub.docker.com/r/mauricenino/dashdot),
and are available for both AMD64 and ARM devices.

```bash
docker container run -it \
  -p 80:3001 \
  -v /etc/os-release:/etc/os-release:ro \
  -v /proc/1/ns/net:/mnt/host_ns_net:ro \
  --privileged \
  mauricenino/dashdot
```

To get more information on why which flag is needed, or if you want to use other
install options instead (`docker-compose`, or from source), have a look at the [INSTALL.md](./INSTALL.md).

To read more about configuration options, you can visit the [CONFIGURATION.md](./CONFIGURATION.md).
