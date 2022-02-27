Heroku buildpack: Android
=======================

This is an Android [Heroku buildpack](http://devcenter.heroku.com/articles/buildpacks).

Usage
-----

Example usage:

    $ ls
    app/build.gradle

    $ heroku create --stack cedar --buildpack https://gitlab.futurehax.com/FutureHax/androidbuildpack.git

    $ git push heroku master
    ...
    -----> Heroku receiving push
    -----> Fetching custom buildpack
    -----> Android Gradle app detected
    -----> Found a build.gradle

The buildpack will detect that your app has an `/app/build.gradle` in the root. If this file has contents, The Android SDK will be installed and configured.