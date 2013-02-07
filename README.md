# Guard::Cane
[![Build Status](https://secure.travis-ci.org/justincampbell/guard-cane.png)](https://secure.travis-ci.org/justincampbell/guard-cane)
[![Gem Version](https://badge.fury.io/rb/guard-cane.png)](http://badge.fury.io/rb/guard-cane)

Guard::Cane automatically runs [Cane](https://github.com/square/cane#usage)
when files change.

## Installation

Put this in your Gemfile:

```rb
gem 'guard-cane'
```

And then install with:

```sh
$ bundle
$ guard init cane
```

This will place the following in your Guardfile:

```rb
guard :cane, cli: "--color" do
  watch(/.*\.rb/) 
end
```

Also recommended is adding a `.cane` file to your project. See
[square/cane](https://github.com/square/cane#usage) for details.

