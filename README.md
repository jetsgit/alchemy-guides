The Alchemy CMS Guidelines [![Build Status](https://travis-ci.org/AlchemyCMS/alchemy-guides.svg?branch=master)](https://travis-ci.org/AlchemyCMS/alchemy-guides)
==========================

The master branch covers the Alchemy CMS edge version.

Please check out the other branches for guides for the latest stable or older versions of Alchemy CMS.

The guides are created with the [guides](https://github.com/AlchemyCMS/guides) gem and are written in [textile](http://redcloth.org/textile) or [markdown](http://daringfireball.net/projects/markdown/syntax) markup.

## File locations

The top level namespace includes the top level static welcome page of http://guides.alchemy-cms.com.

The actual guides live in the `/guides` folder.

## Preview the guides

**In the `/guides` folder:**

Run

```sh
bundle install
```

to install [guides](https://github.com/AlchemyCMS/guides).

To run a local guides server, run

```sh
bundle exec guides preview
```

The server will be available at [0.0.0.0:9292](http://0.0.0.0:9292).

## Building

Build the guides html files with:

```sh
./build.sh
```

## Deployment

Deploy the files via:

```sh
bundle exec cap deploy
```

**Deployment takes care of the version deployed.** So, if you want to deploy the 3.3 guides you need to checkout the `3.3` branch first.

The `master` branch deploys the edge version.

## Contributing

1. Fork it
2. Create a branch (`git checkout -b my-new-guide`)
3. Commit your changes (`git commit -am 'Add new guide for elements'`)
4. Push to the branch (`git push origin my-new-guide`)
5. Create new Pull Request
