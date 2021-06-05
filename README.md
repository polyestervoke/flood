# Flood Saber's Fork

Forked from [flood](https://github.com/jesec/flood), credits to [jesec](https://github.com/jesec). The goal is to replace rutorrent, with following changes:

- Save torrent file as human name instead of hash name: [PR](https://github.com/sabersalv/flood/pull/3), [Discussion](https://github.com/jesec/flood/pull/316)
- Change cookie SameSite from Strict to Lax: [PR](https://github.com/sabersalv/flood/pull/4), [Discussion](https://github.com/jesec/flood/pull/318)

## Install

- Docker Image: [sabersalv/flood](https://hub.docker.com/r/sabersalv/flood/)

## Release

```
vi package.json
  "version": 1.0.0
git tag v1.0.0
git push --tags
```

