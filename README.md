## Sensu-Plugins-victorops

[![Build Status](https://travis-ci.org/sensu-plugins/sensu-plugins-victorops.svg?branch=master)](https://travis-ci.org/sensu-plugins/sensu-plugins-victorops)
[![Gem Version](https://badge.fury.io/rb/sensu-plugins-victorops.svg)](http://badge.fury.io/rb/sensu-plugins-victorops)
[![Code Climate](https://codeclimate.com/github/sensu-plugins/sensu-plugins-victorops/badges/gpa.svg)](https://codeclimate.com/github/sensu-plugins/sensu-plugins-victorops)
[![Test Coverage](https://codeclimate.com/github/sensu-plugins/sensu-plugins-victorops/badges/coverage.svg)](https://codeclimate.com/github/sensu-plugins/sensu-plugins-victorops)
[![Dependency Status](https://gemnasium.com/sensu-plugins/sensu-plugins-victorops.svg)](https://gemnasium.com/sensu-plugins/sensu-plugins-victorops)

## Functionality

## Files
 * bin/handler-victorops

## Usage

```
{
  "victorops": {
    "api_url": "YOUR_API_URL_WHITOUT_ROUTING_KEY",
    "routing_key": "everyone"
  }
}
```
## Installation

Add the public key (if you haven’t already) as a trusted certificate

```
gem cert --add <(curl -Ls https://raw.githubusercontent.com/sensu-plugins/sensu-plugins.github.io/master/certs/sensu-plugins.pem)
gem install sensu-plugins-victorops -P MediumSecurity
```

You can also download the key from /certs/ within each repository.

#### Rubygems

`gem install sensu-plugins-victorops`

#### Bundler

Add *sensu-plugins-disk-checks* to your Gemfile and run `bundle install` or `bundle update`

#### Chef

Using the Sensu **sensu_gem** LWRP
```
sensu_gem 'sensu-plugins-victorops' do
  options('--prerelease')
  version '0.0.1'
end
```

Using the Chef **gem_package** resource
```
gem_package 'sensu-plugins-victorops' do
  options('--prerelease')
  version '0.0.1'
end
```

## Notes
