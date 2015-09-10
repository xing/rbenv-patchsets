# rbenv-railsexpress

This repository contains the rbenv (ruby-build) build instructions for the
railsexpress patched versions of ruby.

## USAGE

Install the necessary binaries with homebrew first:

- `brew install rbenv`
- `brew install rbenv-aliases`
- `brew install ruby-build`

Then you can clone this repository with `git clone https://source.xing.com/seo-team/rbenv-railsexpress.git`.
Then you can install a railsexpressed version of ruby with a command like this:

```
RUBY_BUILD_DEFINITIONS=~/xing/support/rbenv-railsexpress rbenv install 2.2.3-railsexpress
rbenv alias --auto
```

This assumes that you have cloned the rbenv-railsexpress to
`~/xing/support/rbenv-railsexpress`. If you have cloned it into a different
location use that location instead.
We suggest to also configure the environment variable in your .bashrc or .zshrc
to allow you to do the `rbenv install` without setting the environment variable
everytime:

```
export RUBY_BUILD_DEFINITIONS=~/xing/support/rbenv-railsexpress
```
