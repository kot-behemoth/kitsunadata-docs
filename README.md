# Kitsuna Data Website

This is the landing page / docs for the [Kitsuna Data](https://github.com/kot-behemoth/kitsunadata) data platform.

## Deployment using Dokku

These are run on the host.

``` sh
# usually your key is already available under the current user's `~/.ssh/authorized_keys` file
cat ~/.ssh/authorized_keys | dokku ssh-keys:add admin

dokku apps:create docs
dokku app-json:set docs appjson-path .dokku/docs.app.json
dokku domains:set docs kitsunadata.com

# Install Let's Encrypt plugin (required by metabase app.json)
dokku plugin:install https://github.com/dokku/dokku-letsencrypt.git

dokku letsencrypt:set docs email greg@goltsov.info
dokku letsencrypt:enable docs

# Add Dokku as a remote to your Git repository
git remote add dokku-docs dokku@kitsunadata.com:docs
git push dokku-docs main
```
