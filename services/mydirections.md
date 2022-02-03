# My personal directions request

First, explore the various options through the Directions API https://developers.google.com/maps/documentation/directions/get-directions. 

Be creative and use multiple parameters from the API documentation to earn a top grade. The rubric is listed in the bottom of the MarkDown document. 

> Tip: Can't make changes? GitHub previews MD documents by default (read-only). Start editing to make the changes for your URL and JSON response below

## Directions URL

```
https://maps.googleapis.com/maps/api/directions/json?origin=place_id:ChIJH4BzrwX0K4gR2w0LqfwQcwI&destination=place_id:ChIJhUlGD9D1K4gR7Jad7d1UXCU&mode=bicycling&waypoints=place_id:ChIJRwHNEz71K4gRaLBOj-x889Y|place_id:ChIJodTTig30K4gRIHD1jB1vAt8&key=AIzaSyCM-WWHYHIKY-do4kquMy9Z4wQaQx51AuE&arrival_time=1644091539&units=imperial
```
This URL represents a saturday afternoon bike Ride around Waterloo.  It has seven query string parameters:

- The origin location:  origin=[place_id:ChIJH4BzrwX0K4gR2w0LqfwQcwI](https://www.google.com/maps/search/?api=1&query=Waterloo%20Park&query_place_id=ChIJH4BzrwX0K4gR2w0LqfwQcwI)  
- The destination location:  destination=[place_id:ChIJhUlGD9D1K4gR7Jad7d1UXCU](https://www.google.com/maps/search/?api=1&query=Lady%20Glaze%20Doughnuts&query_place_id=ChIJhUlGD9D1K4gR7Jad7d1UXCU)  
- The mode of transportation:  mode=bicycling  
- Intermediate stops:  waypoints=[place_id:ChIJRwHNEz71K4gRaLBOj-x889Y](https://www.google.com/maps/search/?api=1&query=Four%20All%20Ice%20Cream%20Scoop%20Shop&query_place_id=ChIJRwHNEz71K4gRaLBOj-x889Y)|[place_id:ChIJodTTig30K4gRIHD1jB1vAt8](https://www.google.com/maps/search/?api=1&query=Canadian%20Clay%20and%20Glass%20Gallery&query_place_id=ChIJodTTig30K4gRIHD1jB1vAt8)
- The API Key:  key=AIzaSyCM-WWHYHIKY-do4kquMy9Z4wQaQx51AuE  
- The desired arrival time:  arrival_time=1644091539  
- The units of measurement (feet/miles):  units=imperial  


## Next paste the full JSON response to this query here:

```JSON
PASTE_YOUR_JSON_RESULTS_HERE
```
____
## Rubric

This is part of your first practical lab in Week 3 

1. A working URL properly documented in the MarkDown with a unique origin and destination earns 50%
2. Including one to four additional functioning unique parameters from the API earns 50-70%
3. Having 3 or more functioning unique/novel and well-thought out parameters from the API earns 70-90%
4. Including more than 2 "stops", including links to display PlaceIDs on Google Maps, or other innovative presentations earns 80%-100%. 
