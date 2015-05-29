EGO Theme For Discourse
=====================

1. SSH into your server.

2. `cd /var/discourse`

3. Open `containers/app.yml` and make the following changes:

  1. Add the git clone of this plugin to the plugin list under `hooks:` below the Discourse Docker Manager plugin like so: `- git clone https://github.com/SGColdSun/ego-base.git`

  2. Exit and save changes

4. Run `./launcher rebuild app` to apply the changes.