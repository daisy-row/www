## Hosting a local copy of this website

### Setup

```bash
gem install bundler
git clone --recursive git@github.com:dstebila/oqs-www-new
cd oqs-www-new
bundle install
```

### Building the website

You can build a copy of the website into the `_site` directory by running

```bash
bundle exec jekyll build
```

Alternatively, you can have Jekyll launch a process which will (a) serve the website on a local port, and (b) rebuild whenever a file on disk changes:

```bash
bundle exec jekyll serve
```

The output will show the local address that the web server is running on.

Note that `jekyll serve` doesn't seem to pick up some changes, such as changes to the `_config.yml` site configuration file, or if you have a custom plugin (which we don't).
