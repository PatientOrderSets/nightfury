[![Stories in Ready](https://badge.waffle.io/avinasha/nightfury.png)](http://waffle.io/avinasha/nightfury)

# Nightfury

## Concept

Nightfury provides a reporting framework built on Redis for Ruby/Ruby on Rails applications. The framework is designed 
to store different metrics in a time series or as a single value which can be easily queried. 
The following are the key terms:

### Identity

A identity is an entity for which you want to store reports.

* In a ticketing system this might be `Company` or a `Ticket` or an `Agent`
* Has an id (can auto-generate but generally provided so you can map it to your db ids etc)
* Has metrics

### Metrics

An identity has many metrics.

* Metric can be a single value or a time series. 
* The value can be aggregate (average)

### Tags

Identities can be tagged and have multiple tags.
You can ask for stats for identities with certain tags over a particular time range (if the metric is a series)

## Usage

**See example.rb for usage**

## Installation

Add this line to your application's Gemfile:

    gem 'nightfury'

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install nightfury

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Added some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request
