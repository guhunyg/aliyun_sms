# AliyunSms

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'aliyun_sms'
```

And then execute:

$ bundle

Or install it yourself as:

$ gem install aliyun_sms

## Usage

### 1.Configure first

``` ruby
AliyunSms.configure do |config|

  config.access_key_id = 'testid'
  config.access_key_secret = 'testsecret'

# config.format = "XML"   ## optional(default 'JSON')
# config.region_id = "cn-hangzhou"  ## optional

end
```

### 2.Send a message

``` ruby
  args = {:phone=>"123456789",:sign_name=>"标签测试", :tpl_id=>"SMS_1650053", :params=>{"code":"1234"}}
  AliyunSms.to args
```

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/[USERNAME]/aliyun_sms. This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [Contributor Covenant](http://contributor-covenant.org) code of conduct.


## License

The gem is available as open source under the terms of the [MIT License](http://opensource.org/licenses/MIT).

