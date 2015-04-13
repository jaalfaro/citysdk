# Global





* * *

## Class: CitySDK
Instantiates an instance of the CitySDK object.

**stateCapitals**: `object` , Dictionary of state codes to state capital coordinates. i.e. "AL" -> 32.3617, -86.2792
**apis**: `object` , Available apis and their related functions
**aliases**: `object` , Dictionary of aliases, string alias -> object with variable and description
**acs5years**: `object` , ACS5 available years and the apis available with those years
### CitySDK.ajaxRequest(url) 

Makes an AJAX call

**Parameters**

**url**: `string`, URL to request

**Returns**: `promise`, Returns a standard ajax promise

### CitySDK.jsonpRequest(url) 

Makes an AJAX call (using jsonp)

**Parameters**

**url**: `string`, URL to request

**Returns**: `object`, Returns a standard ajax promise

### CitySDK.latLngToFIPS(lat, lng, callback) 

Converts co-ordinates to Census FIPS via the Geocoder API

**Parameters**

**lat**: `float`, Latitude

**lng**: `float`, Longitude

**callback**: `function`, Callback function


### CitySDK.acs5SummaryRequest(request, callback) 

Makes a request to the ACS5 Summary API. Should be used via APIRequest and not on its own, typically

**Parameters**

**request**: `object`, JSON request (see APIRequest)

**callback**: `function`, Makes a request to the ACS5 Summary API. Should be used via APIRequest and not on its own, typically


### CitySDK.parseToVariable(aliasOrVariable) 

Checks to see if a string is in the aliases dictionary and returns the appropriate variable if so.

**Parameters**

**aliasOrVariable**: `string`, A string to parse into a variable string.

**Returns**: `string`, Variable string

### CitySDK.APIRequest(request, callback) 

Processes a data request by looking at a JSON request

**Parameters**

**request**: `object`, The JSON object of the request

**callback**: `function`, A callback, which accepts a response parameter


### CitySDK.GEORequest(request, callback) 

Get a city's geography by name, as well as requested variables

**Parameters**

**request**: `object`, The JSON request

**callback**: `function`, The callback to take the response, which is geoJSON




* * *









