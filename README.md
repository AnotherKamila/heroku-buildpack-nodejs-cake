Heroku Buildpack for Node.js + Pre-launch tasks
===============================================

Forked from the original [Heroku nodejs buildpack](https://github.com/heroku/heroku-buildpack-nodejs), this buildpack adds a last step of calling `cake pre-launch`, thereby allowing for additional build steps such as bundling client-side javascript. (It also installs `devDependencies`, as my random guess is that that is where build-dependencies should go...)

To switch to this build pack in an app:

    heroku config:set BUILDPACK_URL=https://github.com/AnotherKamila/heroku-buildpack-nodejs-cake
