# yt-fanfinder

This is a sample project sample that illustrates how one could recreate the
YouTube Fan Finder web site (http://www.youtube.com/yt/fanfinder/) in the Grow SDK.

For full documentation on Grow, visit: http://growsdk.org

Here's a quick codelab that shows off some of the capabilities of Grow SDK:

    # Downloads the pod from GitHub to a directory "yt-fanfinder".
    grow init https://github.com/jeremydw/growsdk-sample-yt-fanfinder.git yt-fanfinder

    cd yt-fanfinder

    # Creates machine translations for three locales (ar, de, ja).
    grow machine_translate --locale=ar --locale=de --locale=ja .

    # Start the development server (default port is 8080).
    grow run .

    # Now visit http://localhost:8080/yt/fanfinder/ to see your pod.
    # Use Ctrl+C to shut down the server.

    # Deploys the site to a directory "yt-fanfinder-build" (configured in podspec.yaml).
    grow deploy .

Once you've run through the commands, you can play with the configs in the `/content/`
folder and the `/podspec.yaml` file. Note that this is just a simple one-page site, and
it does not illustrate the capabilities of the Sass or Closure preprocessor.

It does, however, come with translations and shows off how to build a multilingual
language select menu automatically.

This pod was derived from HTML available at http://www.youtube.com/yt/fanfinder/ and produces
a site that links to files hosted on on youtube.com. If the files disappear, this site
will not function properly.
