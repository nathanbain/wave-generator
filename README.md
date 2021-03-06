# WAVE GENERATOR

_Accessibility reports from your command line!_

Wave Generator will generate an accessibility report for your website using the Wave Plugin for Firefox.

Example:

```ruby

rake wave:make_errors                                                                                                                                         

Wave Accessibility Report - Showing Errors Only

* ERROR: Form label missing: A form <input>, <select>, or <textarea> does not have a corresponding label. (Note: Labels are not required for image, submit, reset, button, or hidden form element types.).

Summary: Errors (1)

```

## Prerequisites

* [Ruby](http://www.ruby-lang.org/en/)
* [Rubygems](http://rubygems.org/pages/download)
* [Bundler](http://gembundler.com/)
* [Firefox](http://www.mozilla.org/en-US/firefox/all/)

## Installation

* Clone this project `git clone https://github.com/nathanbain/wave-generator.git`
* Run `bundle install`
* Run the rake task `rake wave:make URL=<your-websites-url>`

## Rake Tasks

* Default - `rake wave:make URL=<your-websites-url>` - Reports Errors, Features and Others.
* Errors + Features - `rake wave:make_errors_and_features URL=<your-websites-url>` - Reports Errors and Features only.
* Errors - `rake wave:make_errors URL=<your-websites-url>` - Reports Errors only.
