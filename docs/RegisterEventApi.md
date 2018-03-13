# SwaggerClient::RegisterEventApi

All URIs are relative to *http://166.70.118.105:8986/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**add_event**](RegisterEventApi.md#add_event) | **POST** /register_event | Register a new event
[**update_event**](RegisterEventApi.md#update_event) | **POST** /update_event | Register a new event


# **add_event**
> add_event(body)

Register a new event



### Example
```ruby
# load the gem
require 'swagger_client'

api_instance = SwaggerClient::RegisterEventApi.new

body = SwaggerClient::Event.new # Event | Event object that needs to be added to the Index


begin
  #Register a new event
  api_instance.add_event(body)
rescue SwaggerClient::ApiError => e
  puts "Exception when calling RegisterEventApi->add_event: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**Event**](Event.md)| Event object that needs to be added to the Index | 

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



# **update_event**
> update_event(body)

Register a new event



### Example
```ruby
# load the gem
require 'swagger_client'

api_instance = SwaggerClient::RegisterEventApi.new

body = SwaggerClient::Event.new # Event | Event object that needs to be added to the Index


begin
  #Register a new event
  api_instance.update_event(body)
rescue SwaggerClient::ApiError => e
  puts "Exception when calling RegisterEventApi->update_event: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**Event**](Event.md)| Event object that needs to be added to the Index | 

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



