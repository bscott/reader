# Reader [![Build Status](https://travis-ci.org/amrnt/reader.png?branch=master)](https://travis-ci.org/amrnt/reader) [![Code Climate](https://codeclimate.com/badge.png)](https://codeclimate.com/github/amrnt/reader)

A tool to read a link and extracts its data.

## Usage

After installing the gem you are ready to go. For now I'm implementing Techcrunch.com

```ruby
tc = Reader::Techcrunch 'http://techcrunch.com/...'
tc.title   # Article Title
tc.body    # Article body
tc.as_hash # { :title => "...", :body => "..." }
tc.as_json # "{\"title\": \"...\", \"body\": \"...\"}"
```

### Available Providers

* `Reader::Techcrunch`: `title, body`
* `Reader::Mashable`: `title, body`
* `Reader::Medium`: `title, body, author, publish_date`

## Installation

Add this line to your application's Gemfile:

    gem 'reader'

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install reader

## TODO

* Wrtie more tests
* implement more Websites
* 
