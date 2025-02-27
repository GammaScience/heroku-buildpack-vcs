# heroku-buildpack-vcs

Add support for worker requiring vcs systems


Heroku Buildpack: Version Control Systems
=====================

Add `git` support and possibly other VCS in due course.


Usage
-----

Set `GIT_CONFIG` variable to private key:

    heroku config:set GIT_CONFIG="`cat /path/to/.gitconfig`"


Enable the multi buildpack:

    heroku config:set BUILDPACK_URL=https://github.com/ddollar/heroku-buildpack-multi.git

Create `.buildpacks` file:

    https://github.com/${YOUR_NAME}/heroku-buildpack-vcs.git
    ssh://git@github.com:${YOUR_NAME}/top-secret-buildpack.git
    https://github.com/heroku/heroku-buildpack-something-something.git


It is highly recommended that you use your own fork as updates may break backwards compatibility.


Bugs
----

Please report any bugs to using the [issue tracker](https://github.com/GammaScience/heroku-buildpack-vcs/issues).

Pull requests are welcome.