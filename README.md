# UrlValidator

[![Build Status](https://img.shields.io/travis/riboseinc/url_validator/master.svg)](https://travis-ci.org/riboseinc/url_validator)

Validate URL formats in ActiveModels.

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'url_validator'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install url_validator

## Usage

Add the following to your model:

```ruby
validates :my_url_attribute, url: true
```

## Error messages

You can set the error message as an additional parameter

```ruby
validates :my_url_attribute, url: true, message: 'is not a valid URL'
```

or you can use locales:

```yaml
en:
  errors:
    messages:
      invalid_url: 'is not a valid URL'
```

## Development

After checking out the repo, run `bin/setup` to install dependencies. Then, run 
`rake spec` to run the tests. You can also run `bin/console` for an interactive 
prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To 
release a new version, update the version number in `version.rb`, and then run 
`bundle exec rake release`, which will create a git tag for the version, push 
git commits and tags, and push the `.gem` file to 
[rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at 
https://github.com/riboseinc/url_validator. This project is intended to be a 
safe, welcoming space for collaboration, and contributors are expected to 
adhere to the [Contributor Covenant](http://contributor-covenant.org) code of 
conduct.


## License

The gem is available as open source under the terms of the [MIT 
License](http://opensource.org/licenses/MIT).

