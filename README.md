Marine Weather API
============

Marine Weather is a simple tool for getting marine weather data. It returns the current weather conditions in coordinates within the ocean and sea.

![Build Status](https://img.shields.io/badge/build-passing-green)
![Code Climate](https://img.shields.io/badge/maintainability-B-purple)
![Prod Ready](https://img.shields.io/badge/production-ready-blue)

This is a Python API Wrapper for the [Marine Weather API](https://apiverve.com/marketplace/api/marineweather)

---

## Installation
	pip install apiverve-marineweather

---

## Configuration

Before using the marineweather API client, you have to setup your account and obtain your API Key.  
You can get it by signing up at [https://apiverve.com](https://apiverve.com)

---

## Usage

The Marine Weather API documentation is found here: [https://docs.apiverve.com/api/marineweather](https://docs.apiverve.com/api/marineweather).  
You can find parameters, example responses, and status codes documented here.

### Setup

```
# Import the client module
from apiverve_marineweather.apiClient import MarineweatherAPIClient

# Initialize the client with your APIVerve API key
api = MarineweatherAPIClient("[YOUR_API_KEY]")
```

---


### Perform Request
Using the API client, you can perform requests to the API.

###### Define Query

```
query = { "lat": 29.48003,  "lon": -37.62424 }
```

###### Simple Request

```
# Make a request to the API
result = api.execute(query)

# Print the result
print(result)
```

###### Example Response

```
{
  "status": "ok",
  "error": null,
  "data": {
    "location": {
      "lat": 29.48003,
      "lon": -37.62424
    },
    "weather": {
      "maxtempc": 26.1,
      "maxtempf": 79,
      "mintempc": 21.7,
      "mintempf": 71.1,
      "avgtempc": 25.4,
      "avgtempf": 77.8,
      "maxwindmph": 12,
      "maxwindkph": 19.3,
      "totalprecipmm": 2.36,
      "totalprecipin": 0.09,
      "totalsnowcm": 0,
      "avgviskm": 9.5,
      "avgvismiles": 5,
      "moonphase": "New Moon",
      "moonillumination": 0
    }
  },
  "code": 200
}
```

---

## Customer Support

Need any assistance? [Get in touch with Customer Support](https://apiverve.com/contact).

---

## Updates
Stay up to date by following [@apiverveHQ](https://twitter.com/apiverveHQ) on Twitter.

---

## Legal

All usage of the APIVerve website, API, and services is subject to the [APIVerve Terms of Service](https://apiverve.com/terms) and all legal documents and agreements.

---

## License
Licensed under the The MIT License (MIT)

Copyright (&copy;) 2025 APIVerve, and EvlarSoft LLC

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.