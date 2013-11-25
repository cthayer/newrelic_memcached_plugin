## New Relic Memcached Extension

Prerequisites
-------------
- A New Relic account. Signup for a free account at [http://newrelic.com](http://newrelic.com)
- A server running Memcached v1.4 or greater. Download the latest version of Memcached for free [here](https://code.google.com/p/memcached/downloads/list).
- Ruby version 1.8.7 or better

Running the Agent
----------------------------------

1. Download the latest `newrelic_memcached_plugin-X.Y.Z.tar.gz` from [the tags list](https://github.com/newrelic-platform/newrelic_memcached_plugin/tags)
1. Extract the downloaded archive to the location you want to run the Memcached agent from
1. Run `bundle install` to install required gems
1. Copy `config/template_newrelic_plugin.yml` to `config/newrelic_plugin.yml`
1. Edit `config/newrelic_plugin.yml` to point to your instances of Memcached. You can add as many hosts as you'd like If your Memcached instances are bound to an external IP, use that value for the host field.  If you omit the 'port' field it will default to '11211'
1. Edit the `config/newrelic_plugin.yml` file by changing the name and endpoint fields to match your Memcached server configuration
1. From your shell run: `./newrelic_memcached_agent`
1. Wait a few minutes for New Relic to begin processing the data sent from your agent.
1. Log into your New Relic account at [http://newrelic.com](http://newrelic.com) and click on `Memcached` on the left hand nav bar to start seeing your Memcached metrics

Source Code
-----------

This plugin can be found at [https://github.com/newrelic-platform/newrelic_memcached_plugin](https://github.com/newrelic-platform/newrelic_memcached_plugin)