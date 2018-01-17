
# Nativescript Google Places Autocomplete

Add location autocomplete to your Nativescript application

## Prerequisites 

Create and grap your Api key from  [https://developers.google.com/maps/documentation/javascript/get-api-key?hl=en](https://developers.google.com/maps/documentation/javascript/get-api-key?hl=en)

## Installation

```javascript
tns plugin add nativescript-google-places-autocomplete
```

## Usage 
	
	```javascript
    import { GooglePlacesAutocomplete } from 'nativescript-google-places-autocomplete';
	
	let API_KEY = "your_api_Key";
	let googlePlacesAutocomplete = new GooglePlacesAutocomplete(API_KEY);

	googlePlacesAutocomplete.search(params)
	      .then((places: any) => {
		      // place predictions list
           }, (error => {
              console.log(error)
          }));
          
	googlePlacesAutocomplete.getPlaceById(place.placeId).then((place) => {
	   .then(function () { });
        }, error => {
            console.log(error)
        })        
    ```
    Plugin Auther : [Aymen Labidi](https://aymen.co)

    
## License

Apache License Version 2.0, January 2004
