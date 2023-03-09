# Flood Saber's Fork

> [Original README](./README.original.md), forked from [jesec/flood](https://github.com/jesec/flood)

The goal is to replace rutorrent, with following changes:

- Save torrent file as human name instead of hash name: [PR](https://github.com/sabersalv/flood/pull/3)
- Change cookie SameSite from Strict to Lax: [PR](https://github.com/sabersalv/flood/pull/4)
- Can use freeleech token on RSS feed: [PR](https://github.com/sabersalv/flood/pull/5)
- Display selected count and size on action bar: [PR](https://github.com/sabersalv/flood/pull/9)
- Select all button on action bar: [PR](https://github.com/sabersalv/flood/pull/10)
- Click to play video: [PR](https://github.com/sabersalv/flood/pull/11)

## Install

- Docker Image: [sabersalv/flood](https://hub.docker.com/r/sabersalv/flood/)

## Development

```
brew install rtorrent
npm install
npm run build
npm run start:development:client
npm run start:development:server
rtorrent -o network.scgi.open_local=/tmp/rtorrent.sock
```

## Release

```
npm run build     # outputs no error
vi package.json
  "version": "1.0.0-1"
git tag v1.0.0-1
git push --tags
Github Actions will build and publish to Docker Hub
```
