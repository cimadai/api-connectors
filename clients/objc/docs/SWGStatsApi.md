# SWGStatsApi

All URIs are relative to *https://localhost/api/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**statsGet**](SWGStatsApi.md#statsget) | **GET** /stats | Get exchange-wide and per-series turnover and volume statistics.
[**statsHistory**](SWGStatsApi.md#statshistory) | **GET** /stats/history | Get historical exchange-wide and per-series turnover and volume statistics.


# **statsGet**
```objc
-(NSNumber*) statsGetWithCompletionHandler: 
        (void (^)(NSArray<SWGStats>* output, NSError* error)) handler;
```

Get exchange-wide and per-series turnover and volume statistics.

### Example 
```objc


SWGStatsApi*apiInstance = [[SWGStatsApi alloc] init];

// Get exchange-wide and per-series turnover and volume statistics.
[apiInstance statsGetWithCompletionHandler: 
          ^(NSArray<SWGStats>* output, NSError* error) {
                        if (output) {
                            NSLog(@"%@", output);
                        }
                        if (error) {
                            NSLog(@"Error calling SWGStatsApi->statsGet: %@", error);
                        }
                    }];
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**NSArray<SWGStats>***](SWGStats.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **statsHistory**
```objc
-(NSNumber*) statsHistoryWithCompletionHandler: 
        (void (^)(NSArray<SWGStatsHistory>* output, NSError* error)) handler;
```

Get historical exchange-wide and per-series turnover and volume statistics.

### Example 
```objc


SWGStatsApi*apiInstance = [[SWGStatsApi alloc] init];

// Get historical exchange-wide and per-series turnover and volume statistics.
[apiInstance statsHistoryWithCompletionHandler: 
          ^(NSArray<SWGStatsHistory>* output, NSError* error) {
                        if (output) {
                            NSLog(@"%@", output);
                        }
                        if (error) {
                            NSLog(@"Error calling SWGStatsApi->statsHistory: %@", error);
                        }
                    }];
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**NSArray<SWGStatsHistory>***](SWGStatsHistory.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

