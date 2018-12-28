# rbenv-railsexpress

This repository contains the rbenv (ruby-build) build instructions for the railsexpress patched versions of ruby.

## Usage

Install rbenv and plugins using homebrew:

```sh
brew install rbenv
brew install rbenv-aliases
brew install ruby-build
```

Install this plugin:

```sh
git clone https://github.com/xing/rbenv-patchsets.git ~/.rbenv/plugins/ruby-build-railsexpress
```

Install railsexpress version:

```sh
rbenv install 2.5.1-railsexpress
```

`rbenv alias --auto` creates an alias `2.5.1` for `2.5.1-railsexpress`

## Troubleshooting

On OSX El Capitan it can happen that gems fail to build because of openssl errors.
The following command might help:

```sh
gem install eventmachine -v '1.0.8' -- --with-cppflags=-I/usr/local/opt/openssl/include
```

## Update definitions

Just run update script in the plugin directory:

```sh
cd ~/.rbenv/plugins/ruby-build-railsexpress
./update
```
