# PeakflowUtils

Various tools to use with www.peakflow.io.

## Installation
Add this line to your application's Gemfile:

```ruby
gem "peak_flow_utils"
```

And then execute:
```bash
$ bundle
```

Or install it yourself as:
```bash
$ gem install peak_flow_utils
```

Add this to `config/peakflow.rb`:
```ruby
PeakFlowUtils::Notifier.configure(auth_token: "your-token")
```

## Usage

### Reporting errors manually

```ruby
PeakFlowUtils::Notifier.notify(error: error)
```

### Reporting Rails errors

Add this to `config/peakflow.rb`:
```ruby
PeakFlowUtils::NotifierRails.configure
```

### Reporting Sidekiq errors in Rails:

Add this to `config/peakflow.rb`:
```ruby
PeakFlowUtils::NotifierSidekiq.configure
```

## Contributing
Contribution directions go here.

## License
The gem is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).
