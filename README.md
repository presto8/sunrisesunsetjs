SunriseSunsetJS Class
===================

Overview
--------

Implementation of http://williams.best.vwh.net/sunrise_sunset_algorithm.htm

Provides sunrise and sunset times for a specified date and position.
All dates are UTC. Year is 4-digit. Month is 1-12. Day is 1-31.
Longitude is positive for east, negative for west. Latitude is
positive for north, negative for south.

Sample Usage
------------

```javascript
var tokyo = new SunriseSunset( 2011, 1, 19, 35+40/60, 139+45/60); 
tokyo.sunriseUtcHours()      --> 21.8199 = 21:49 GMT
tokyo.sunsetUtcHours()       --> 7.9070  = 07:54 GMT
tokyo.sunriseLocalHours(9)   --> 6.8199  = 06:49 at GMT+9
tokyo.sunsetLocalHours(9)    --> 16.9070 = 16:54 at GMT+9
tokyo.isDaylight(1.5)        --> true

var losangeles = new SunriseSunset( 2011, 1, 19, 34.05, -118.233333333 );
```

License
-------

Copyright 2011-2013 Preston Hunt <me@prestonhunt.com>

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
