# Photon Design System  [![Build Status](https://travis-ci.org/FirefoxUX/photon.svg?branch=master)](https://travis-ci.org/FirefoxUX/photon)

Requires:
* docker

To preview your changes (with hot-reloading!):

Check out a copy of the repository, and go to that directory. Then run:
```
$ docker pull praqma/gh-pages
$ docker run --name photon -d -v $PWD/jekyll:/home/jenkins -p 4000:4000 praqma/gh-pages || docker start photon
$ docker exec -it photon jekyll serve --watch --host=0.0.0.0
```
and open up http://localhost:4000/photon/

When you're done, you can hit `ctrl-c` to stop the `docker exec` command, and then run `docker stop` to stop the container.
If you want to resume working on it, you can run:
```
$ docker start photon
$ docker exec -it photon jekyll serve --watch --host=0.0.0.0
```

Once you have something you like, it's time to share it with the rest of us!

To get your changes merged:
* Make sure you're working on `staging`, and submit the pull request to there. All our commits go through the staging site before being pushed to `master`.
* Make your pull request as small as possible (so it's easier to review and merge them).
* If it's something that needs to be merged as soon as possible, add a tag (e.g. urgent).
