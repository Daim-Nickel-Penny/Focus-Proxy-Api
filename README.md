# Focus-Chrome-Home-Extension
[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)

This is an API for a chrome extension, called Focus which shows new background images on every tab.
The api fetches the image from the database and then returns it to the extension.
It is a proxy API.
Too many requests are also handled with a IP lock.

Extension can be found [here](https://github.com/Daim-Nickel-Penny/Focus-Chrome-Extension)

## Caching Enabled
Caching is enabled to improve the performance for every tab if opneded within the new image request time.

## Response for the API is-

```sh
{
    "copyright": "Roberto Colombari",
    "date": "2014-06-30",
    "explanation": "What's happened to the center of this galaxy? Unusual and dramatic dust lanes run across the center of elliptical galaxy Centaurus A. These dust lanes are so thick they almost completely obscure the galaxy's center in visible light.  This is particularly unusual as Cen A's red stars and round shape are characteristic of a giant elliptical galaxy, a galaxy type usually low in dark dust.  Cen A, also known as NGC 5128, is also unusual compared to an average elliptical galaxy because it contains a higher proportion of young blue stars and is a very strong source of radio emission.  Evidence indicates that Cen A is likely the result of the collision of two normal galaxies.  During the collision, many young stars were formed, but details of the creation of Cen A's unusual dust belts are still being researched.  Cen A lies only 13 million light years away, making it the closest active galaxy.  Cen A, pictured above, spans 60,000 light years and can be seen with binoculars toward the constellation of Centaurus.",
    "hdurl": "https://apod./apod/image/1406/CenAwide_colombari_1824.jpg",
    "media_type": "image",
    "service_version": "v1",
    "title": "Peculiar Elliptical Galaxy Centaurus A",
    "url": "https://apod./apod/image/1406/CenAwide_colombari_1824.jpg",
    "cachedTime": 1628172455338
}
```

## Limiter in Action

Blocks the user for 60 seconds before they could again send a request. 
This time can be varyed through code.


![Limiter in action](https://github.com/Daim-Nickel-Penny/Focus-Proxy-Api/blob/main/focuse_img1.PNG?raw=true)
