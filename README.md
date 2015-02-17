## Sensu-Plugins-opentsdb

[![Build Status](https://travis-ci.org/sensu-plugins/sensu-plugins-opentsdb.svg?branch=master)](https://travis-ci.org/sensu-plugins/sensu-plugins-opentsdb)
[![Gem Version](https://badge.fury.io/rb/sensu-plugins-opentsdb.svg)](http://badge.fury.io/rb/sensu-plugins-opentsdb)
[![Code Climate](https://codeclimate.com/github/sensu-plugins/sensu-plugins-opentsdb/badges/gpa.svg)](https://codeclimate.com/github/sensu-plugins/sensu-plugins-opentsdb)
[![Test Coverage](https://codeclimate.com/github/sensu-plugins/sensu-plugins-opentsdb/badges/coverage.svg)](https://codeclimate.com/github/sensu-plugins/sensu-plugins-opentsdb)
[![Dependency Status](https://gemnasium.com/sensu-plugins/sensu-plugins-opentsdb.svg)](https://gemnasium.com/sensu-plugins/sensu-plugins-opentsdb)

## Functionality

## Files
 * bin/handler-opentsdb
 *
 *
 *

## Usage

```
{  
  "opentsdb" : {
     "server" : "opentsdb.int.example.com",
     "port" : 4242,
     "hostname_length" : 3
   }
}
```

## Installation

Add the public key (if you haven’t already) as a trusted certificate

```
gem cert --add <(curl -Ls https://raw.githubusercontent.com/sensu-plugins/sensu-plugins.github.io/master/certs/sensu-plugins.pem)
gem install sensu-plugins-opentsdb -P MediumSecurity
```

You can also download the key from /certs/ within each repository.

#### Rubygems

`gem install sensu-plugins-opentsdb`

#### Bundler

Add *sensu-plugins-disk-checks* to your Gemfile and run `bundle install` or `bundle update`

#### Chef

Using the Sensu **sensu_gem** LWRP
```
sensu_gem 'sensu-plugins-opentsdb' do
  options('--prerelease')
  version '0.0.1'
end
```

Using the Chef **gem_package** resource
```
gem_package 'sensu-plugins-opentsdb' do
  options('--prerelease')
  version '0.0.1'
end
```

## Notes
