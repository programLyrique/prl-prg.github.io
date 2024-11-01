# prl-prg website

# Usage

## Install jekyll (Linux / Windows)

```sh
sudo apt-get install build-essential # if you do not have gcc and stuff
sudo apt-get install ruby ruby-dev   # if you do not have ruby
sudo gem install jekyll bundler      # if you do not have jekyll and bundler
```

## Install jekyll (OSX)

```sh
sudo gem install jekyll bundler      # if you do not have jekyll and bundler
```

## Build the site

```sh
git clone https://github.com/PRL-PRG/prl-prg.github.io.git
cd prl-prg.github.io
bundle install
bundle exec jekyll serve
```

This will run a local webserver. The site is accessible at [localhost:4000](localhost:4000).

Jekyll is not totally compatible with Ruby 3 at the time we write this (Nov. 2022). Running the local webserver will not work 
but you can instead build the website and then open the index page:

```sh
bundle exec jekyll build
open _site/index.html
```

If you have permission problems with `bundle install`, try to do that before:

```bash
export BUNDLE_PATH=~/.gems
```

## Updates

Please test locally and then create a PR.
