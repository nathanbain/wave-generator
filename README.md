# WAVE GENERATOR

_Accessibility reports from your command line!_

Wave Generator will generate an accessibility report for your website using the Wave Plugin for Firefox.

## Prerequisites

* [Ruby](http://www.ruby-lang.org/en/)
* [Rubygems](http://rubygems.org/pages/download)
* [Bundler](http://gembundler.com/)
* [Firefox](http://www.mozilla.org/en-US/firefox/all/)

## Installation

* Clone this project `gem clone https://github.com/nathanbain/wave-generator.git`
* Run `bundle install`
* Run the rake task `rake wave`

## Rake Tasks

* Default - `rake wave` or `rake wave:make` - Reports Errors, Features and Others.
* Default - `rake wave:make_errors_and_features` - Reports Errors and Features only.
* Default - `rake wavemake_errors:` - Reports Errors only.
