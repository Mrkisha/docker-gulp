Gulp
=====

Gulp is `javascript` based task manager. It allows you to compile `js` and `css`. 
Its easy to use, very efficient and easy to learn.

Usage
---

Make sure you have `package.json` file in your host directory that will be mounted as volume to containers directory.

Container's default mounting point is `/tmp/app`.

Run docker command:
```
$ docker run -it -u node --rm -v <host-dir>:<container-dir> gulp sh -c "gulp watch"
```

About this container
---
This container is based on official node image and has installed `Yarn` for package managment.
For now, it does not save `yarn` cache.
However, if you mount volumes, npm packages will be saved to mounting point on the host as all other files including yarn.lock file.

**Current version of `Yarn` is `0.17.10`**

Contributing
---
You are invited to contribute new features, fixes, or updates, large or small; we are always thrilled to receive pull requests, and do our best to process them as fast as we can.

Before you start to code, we recommend discussing your plans through a [GitHub issue](https://github.com/Mrkisha/docker-gulp/issues), especially for more ambitious contributions. This gives other contributors a chance to point you in the right direction, give you feedback on your design, and help you find out if someone else is working on the same thing.
