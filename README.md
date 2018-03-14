# event_client

EventClient - the Ruby gem for the Service API

filters.

- API version: 1.0.0
- Package version: 1.0.0
- Build package: io.swagger.codegen.languages.RubyClientCodegen

## Installation

### Build a gem

To build the Ruby code into a gem:

```shell
gem build event_client.gemspec
```

Then either install the gem locally:

```shell
gem install ./event_client-1.0.0.gem
```
(for development, run `gem install --dev ./event_client-1.0.0.gem` to install the development dependencies)

### Install from Git

If the Ruby gem is hosted at a git repository: https://github.com/zerebral/event_service_client.git, then add the following in the Gemfile:

    gem 'event_client', :git => 'https://github.com/zerebral/event_service_client.git'



## Getting Started

Please follow the [installation](#installation) procedure and then run the following code:
```ruby
# Load the gem
require 'event_client'

api_instance = EventClient::EventApi.new

body = EventClient::Event.new # Event | Event object that needs to be added to the Index


begin
  #Register a new event
  api_instance.add_event(body)
rescue EventClient::ApiError => e
  puts "Exception when calling EventApi->add_event: #{e}"
end

```

## Documentation for API Endpoints

All URIs are relative to *http://166.70.118.105:8986/v1*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*EventClient::EventApi* | [**add_event**](docs/EventApi.md#add_event) | **POST** /register_event | Register a new event
*EventClient::EventApi* | [**update_event**](docs/EventApi.md#update_event) | **POST** /update_event | Register a new event


## Documentation for Models

 - [EventClient::Event](docs/Event.md)


## Documentation for Authorization


### api_key

- **Type**: API key
- **API key parameter name**: api_key
- **Location**: HTTP header

