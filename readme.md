# GIF API

## About GIF API
   GIF API exposes two endpoints to  provided G rated gifs. The first endpoint presents gifs for a specified 
   search term(happy new year, dog). The second endpoint retrieves a specific GIF by the GIF ID.
   The api is HTTP basic authorization protected and can be accessed by providing the username and password.
   This api at the backend invokes GIF API exposed at endpoint http://api.giphy.com

## Development Environment Details
   The api contract is written using specification RAML 1.0, the implementation is done using IDE Anypoint Studio Version 6.5.0. 
   The runtime environment is Mule Server 3.9.0 EE.

## Testing
   Testing of GiF api can be done by api console provided by Mulesoft.
   Once the project is deployed locally, api console is available at http://localhost:8081/console/
   
   Retrive Gif By Tag: 
      URl: http://localhost:8081/api/v1/external/gifs?tag=cat
      Sample Response :
```
         [
  {
      "id" : "3oEjHSUiIjzxqIOo80",
      "description" : "",
      "bitlyGifUrl": "https:\/\/gph.is\/28JoSXz",
      "loopingGifUrl": 
              {
	         "mp4": "https:\/\/media2.giphy.com\/media\/3oEjHSUiIjzxqIOo80\/giphy-loop.mp4",
	         "mp4_size": "503056"
	      } ,
      "creationDateTime" : "2016-06-13 17:41:12",
      "username" : "sesamomx"
  }
]
```
   Retrive Gif By Id: 
      URL:http://localhost:8081/api/v1/external/gifs?id=3oEjHSUiIjzxqIOo80
      Sample Response :
```
 {
      "id" : "3oEjHSUiIjzxqIOo80",
      "description" : "",
      "bitlyGifUrl": "https:\/\/gph.is\/28JoSXz",
      "loopingGifUrl": 
              {
	         "mp4": "https:\/\/media2.giphy.com\/media\/3oEjHSUiIjzxqIOo80\/giphy-loop.mp4",
	         "mp4_size": "503056"
	      }
 }
```

   
   




