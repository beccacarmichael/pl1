# My personal directions request

First, explore the various options through the Directions API https://developers.google.com/maps/documentation/directions/get-directions. 

Be creative and use multiple parameters from the API documentation to earn a top grade. The rubric is listed in the bottom of the MarkDown document. 

> Tip: Can't make changes? GitHub previews MD documents by default (read-only). Start editing to make the changes for your URL and JSON response below

## Directions URL

```
https://maps.googleapis.com/maps/api/directions/json?origin=place_id:ChIJH4BzrwX0K4gR2w0LqfwQcwI&destination=place_id:ChIJhUlGD9D1K4gR7Jad7d1UXCU&mode=bicycling&waypoints=place_id:ChIJodTTig30K4gRIHD1jB1vAt8|place_id:ChIJRwHNEz71K4gRaLBOj-x889Y&key=AIzaSyCM-WWHYHIKY-do4kquMy9Z4wQaQx51AuE&arrival_time=1644091539&units=imperial
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
{
   "geocoded_waypoints" : [
      {
         "geocoder_status" : "OK",
         "place_id" : "ChIJH4BzrwX0K4gR2w0LqfwQcwI",
         "types" : [ "establishment", "park", "point_of_interest", "tourist_attraction" ]
      },
      {
         "geocoder_status" : "OK",
         "place_id" : "ChIJodTTig30K4gRIHD1jB1vAt8",
         "types" : [
            "art_gallery",
            "establishment",
            "museum",
            "point_of_interest",
            "store",
            "tourist_attraction"
         ]
      },
      {
         "geocoder_status" : "OK",
         "place_id" : "ChIJRwHNEz71K4gRaLBOj-x889Y",
         "types" : [ "establishment", "food", "point_of_interest", "store" ]
      },
      {
         "geocoder_status" : "OK",
         "place_id" : "ChIJhUlGD9D1K4gR7Jad7d1UXCU",
         "types" : [ "bakery", "establishment", "food", "point_of_interest", "store" ]
      }
   ],
   "routes" : [
      {
         "bounds" : {
            "northeast" : {
               "lat" : 43.4668588,
               "lng" : -80.518275
            },
            "southwest" : {
               "lat" : 43.45371050000001,
               "lng" : -80.5331345
            }
         },
         "copyrights" : "Map data ©2022 Google",
         "legs" : [
            {
               "distance" : {
                  "text" : "0.7 mi",
                  "value" : 1058
               },
               "duration" : {
                  "text" : "4 mins",
                  "value" : 210
               },
               "end_address" : "25 Caroline St N, Waterloo, ON N2L 2Y5, Canada",
               "end_location" : {
                  "lat" : 43.4649025,
                  "lng" : -80.5256584
               },
               "start_address" : "Waterloo Park, 100 Father David Bauer Dr, Waterloo, ON N2L 2Y4, Canada",
               "start_location" : {
                  "lat" : 43.4657223,
                  "lng" : -80.5331345
               },
               "steps" : [
                  {
                     "distance" : {
                        "text" : "344 ft",
                        "value" : 105
                     },
                     "duration" : {
                        "text" : "1 min",
                        "value" : 19
                     },
                     "end_location" : {
                        "lat" : 43.4650823,
                        "lng" : -80.53244719999999
                     },
                     "html_instructions" : "Head \u003cb\u003esoutheast\u003c/b\u003e toward \u003cb\u003eFather David Bauer Dr\u003c/b\u003e",
                     "polyline" : {
                        "points" : "wkhhG`cpjNBABEBE?GIW?E@EBEbAq@JIJENCJA"
                     },
                     "start_location" : {
                        "lat" : 43.4657223,
                        "lng" : -80.5331345
                     },
                     "travel_mode" : "BICYCLING"
                  },
                  {
                     "distance" : {
                        "text" : "0.1 mi",
                        "value" : 204
                     },
                     "duration" : {
                        "text" : "1 min",
                        "value" : 36
                     },
                     "end_location" : {
                        "lat" : 43.4650763,
                        "lng" : -80.529962
                     },
                     "html_instructions" : "Turn \u003cb\u003eleft\u003c/b\u003e onto \u003cb\u003eFather David Bauer Dr\u003c/b\u003e",
                     "maneuver" : "turn-left",
                     "polyline" : {
                        "points" : "wghhGx~ojNMiCCo@CYCo@AU?c@@]Bc@Ba@F_@Ho@"
                     },
                     "start_location" : {
                        "lat" : 43.4650823,
                        "lng" : -80.53244719999999
                     },
                     "travel_mode" : "BICYCLING"
                  },
                  {
                     "distance" : {
                        "text" : "105 ft",
                        "value" : 32
                     },
                     "duration" : {
                        "text" : "1 min",
                        "value" : 5
                     },
                     "end_location" : {
                        "lat" : 43.46533429999999,
                        "lng" : -80.52996639999999
                     },
                     "html_instructions" : "Turn \u003cb\u003eleft\u003c/b\u003e toward \u003cb\u003eLaurel Trail\u003c/b\u003e",
                     "maneuver" : "turn-left",
                     "polyline" : {
                        "points" : "wghhGfoojNKEIC?AA?A?QBA@A@A@?B"
                     },
                     "start_location" : {
                        "lat" : 43.4650763,
                        "lng" : -80.529962
                     },
                     "travel_mode" : "BICYCLING"
                  },
                  {
                     "distance" : {
                        "text" : "85 ft",
                        "value" : 26
                     },
                     "duration" : {
                        "text" : "1 min",
                        "value" : 4
                     },
                     "end_location" : {
                        "lat" : 43.465535,
                        "lng" : -80.52981149999999
                     },
                     "html_instructions" : "Turn \u003cb\u003eright\u003c/b\u003e toward \u003cb\u003eLaurel Trail\u003c/b\u003e",
                     "maneuver" : "turn-right",
                     "polyline" : {
                        "points" : "iihhGhoojNMIEGEEOG"
                     },
                     "start_location" : {
                        "lat" : 43.46533429999999,
                        "lng" : -80.52996639999999
                     },
                     "travel_mode" : "BICYCLING"
                  },
                  {
                     "distance" : {
                        "text" : "289 ft",
                        "value" : 88
                     },
                     "duration" : {
                        "text" : "1 min",
                        "value" : 15
                     },
                     "end_location" : {
                        "lat" : 43.4660635,
                        "lng" : -80.53061289999999
                     },
                     "html_instructions" : "Turn \u003cb\u003eleft\u003c/b\u003e onto \u003cb\u003eLaurel Trail\u003c/b\u003e",
                     "maneuver" : "turn-left",
                     "polyline" : {
                        "points" : "sjhhGhnojNCJCFILEDKRWb@k@~@"
                     },
                     "start_location" : {
                        "lat" : 43.465535,
                        "lng" : -80.52981149999999
                     },
                     "travel_mode" : "BICYCLING"
                  },
                  {
                     "distance" : {
                        "text" : "0.3 mi",
                        "value" : 482
                     },
                     "duration" : {
                        "text" : "2 mins",
                        "value" : 90
                     },
                     "end_location" : {
                        "lat" : 43.4659778,
                        "lng" : -80.5258571
                     },
                     "html_instructions" : "Turn \u003cb\u003eright\u003c/b\u003e",
                     "maneuver" : "turn-right",
                     "polyline" : {
                        "points" : "{mhhGhsojNGIEE?QEOIKGKGICGACAECQEOESIm@AQ@M@AJe@BIJIFIBG?IAIKYeAmCCEAAA?CACAAAAIAI?ACCGGAIAM@MDOL[NYLWBQ@EDSD_@Da@@G@IDODKHGJGNCZCJGFGBE@G?IGq@"
                     },
                     "start_location" : {
                        "lat" : 43.4660635,
                        "lng" : -80.53061289999999
                     },
                     "travel_mode" : "BICYCLING"
                  },
                  {
                     "distance" : {
                        "text" : "397 ft",
                        "value" : 121
                     },
                     "duration" : {
                        "text" : "1 min",
                        "value" : 41
                     },
                     "end_location" : {
                        "lat" : 43.4649025,
                        "lng" : -80.5256584
                     },
                     "html_instructions" : "Turn \u003cb\u003eright\u003c/b\u003e onto \u003cb\u003eCaroline St N\u003c/b\u003e\u003cdiv style=\"font-size:0.9em\"\u003eDestination will be on the right\u003c/div\u003e",
                     "maneuver" : "turn-right",
                     "polyline" : {
                        "points" : "kmhhGrunjNnCQTALCBARGJE"
                     },
                     "start_location" : {
                        "lat" : 43.4659778,
                        "lng" : -80.5258571
                     },
                     "travel_mode" : "BICYCLING"
                  }
               ],
               "traffic_speed_entry" : [],
               "via_waypoint" : []
            },
            {
               "distance" : {
                  "text" : "0.3 mi",
                  "value" : 413
               },
               "duration" : {
                  "text" : "2 mins",
                  "value" : 120
               },
               "end_address" : "75 King St S Unit 56, Waterloo, ON N2J 1P2, Canada",
               "end_location" : {
                  "lat" : 43.4630135,
                  "lng" : -80.5233166
               },
               "start_address" : "25 Caroline St N, Waterloo, ON N2L 2Y5, Canada",
               "start_location" : {
                  "lat" : 43.4649025,
                  "lng" : -80.5256584
               },
               "steps" : [
                  {
                     "distance" : {
                        "text" : "0.2 mi",
                        "value" : 321
                     },
                     "duration" : {
                        "text" : "2 mins",
                        "value" : 91
                     },
                     "end_location" : {
                        "lat" : 43.4624551,
                        "lng" : -80.52354769999999
                     },
                     "html_instructions" : "Head \u003cb\u003esoutheast\u003c/b\u003e on \u003cb\u003eCaroline St N\u003c/b\u003e toward \u003cb\u003eErb St W\u003c/b\u003e",
                     "polyline" : {
                        "points" : "sfhhGjtnjNDCJILI`@[b@e@VYRSj@g@PMNKl@e@zAkAx@q@bAw@"
                     },
                     "start_location" : {
                        "lat" : 43.4649025,
                        "lng" : -80.5256584
                     },
                     "travel_mode" : "BICYCLING"
                  },
                  {
                     "distance" : {
                        "text" : "144 ft",
                        "value" : 44
                     },
                     "duration" : {
                        "text" : "1 min",
                        "value" : 20
                     },
                     "end_location" : {
                        "lat" : 43.46279579999999,
                        "lng" : -80.52382799999999
                     },
                     "html_instructions" : "Make a \u003cb\u003eU-turn\u003c/b\u003e",
                     "maneuver" : "uturn-left",
                     "polyline" : {
                        "points" : "kwghGdgnjNcAv@"
                     },
                     "start_location" : {
                        "lat" : 43.4624551,
                        "lng" : -80.52354769999999
                     },
                     "travel_mode" : "BICYCLING"
                  },
                  {
                     "distance" : {
                        "text" : "157 ft",
                        "value" : 48
                     },
                     "duration" : {
                        "text" : "1 min",
                        "value" : 9
                     },
                     "end_location" : {
                        "lat" : 43.4630135,
                        "lng" : -80.5233166
                     },
                     "html_instructions" : "Turn \u003cb\u003eright\u003c/b\u003e onto \u003cb\u003eWillis Way\u003c/b\u003e\u003cdiv style=\"font-size:0.9em\"\u003eDestination will be on the left\u003c/div\u003e",
                     "maneuver" : "turn-right",
                     "polyline" : {
                        "points" : "oyghG|hnjNi@eB"
                     },
                     "start_location" : {
                        "lat" : 43.46279579999999,
                        "lng" : -80.52382799999999
                     },
                     "travel_mode" : "BICYCLING"
                  }
               ],
               "traffic_speed_entry" : [],
               "via_waypoint" : []
            },
            {
               "distance" : {
                  "text" : "0.9 mi",
                  "value" : 1451
               },
               "duration" : {
                  "text" : "6 mins",
                  "value" : 346
               },
               "end_address" : "701 Belmont Ave W, Kitchener, ON N2M 1P1, Canada",
               "end_location" : {
                  "lat" : 43.45371050000001,
                  "lng" : -80.518275
               },
               "start_address" : "75 King St S Unit 56, Waterloo, ON N2J 1P2, Canada",
               "start_location" : {
                  "lat" : 43.4630135,
                  "lng" : -80.5233166
               },
               "steps" : [
                  {
                     "distance" : {
                        "text" : "157 ft",
                        "value" : 48
                     },
                     "duration" : {
                        "text" : "1 min",
                        "value" : 7
                     },
                     "end_location" : {
                        "lat" : 43.46279579999999,
                        "lng" : -80.52382799999999
                     },
                     "html_instructions" : "Head \u003cb\u003esouthwest\u003c/b\u003e on \u003cb\u003eWillis Way\u003c/b\u003e toward \u003cb\u003eCaroline St S\u003c/b\u003e/\u003cwbr/\u003e\u003cb\u003eIron Horse Trans Canada Trail\u003c/b\u003e",
                     "polyline" : {
                        "points" : "yzghGvenjNh@dB"
                     },
                     "start_location" : {
                        "lat" : 43.4630135,
                        "lng" : -80.5233166
                     },
                     "travel_mode" : "BICYCLING"
                  },
                  {
                     "distance" : {
                        "text" : "128 ft",
                        "value" : 39
                     },
                     "duration" : {
                        "text" : "1 min",
                        "value" : 5
                     },
                     "end_location" : {
                        "lat" : 43.4630947,
                        "lng" : -80.5240841
                     },
                     "html_instructions" : "Turn \u003cb\u003eright\u003c/b\u003e onto \u003cb\u003eCaroline St S\u003c/b\u003e/\u003cwbr/\u003e\u003cb\u003eIron Horse Trans Canada Trail\u003c/b\u003e",
                     "maneuver" : "turn-right",
                     "polyline" : {
                        "points" : "oyghG|hnjNy@p@"
                     },
                     "start_location" : {
                        "lat" : 43.46279579999999,
                        "lng" : -80.52382799999999
                     },
                     "travel_mode" : "BICYCLING"
                  },
                  {
                     "distance" : {
                        "text" : "0.4 mi",
                        "value" : 631
                     },
                     "duration" : {
                        "text" : "3 mins",
                        "value" : 159
                     },
                     "end_location" : {
                        "lat" : 43.4589585,
                        "lng" : -80.51891289999999
                     },
                     "html_instructions" : "Make a \u003cb\u003eU-turn\u003c/b\u003e at \u003cb\u003eFather David Bauer Dr\u003c/b\u003e\u003cdiv style=\"font-size:0.9em\"\u003eContinue to follow Caroline St S\u003c/div\u003e",
                     "maneuver" : "uturn-left",
                     "polyline" : {
                        "points" : "i{ghGnjnjNx@q@bAw@fDgCLIrA}@LMJQPYr@{Aj@kAlAeCn@uA`@{@DGFEBCBEJSf@cAFMr@wA"
                     },
                     "start_location" : {
                        "lat" : 43.4630947,
                        "lng" : -80.5240841
                     },
                     "travel_mode" : "BICYCLING"
                  },
                  {
                     "distance" : {
                        "text" : "0.1 mi",
                        "value" : 171
                     },
                     "duration" : {
                        "text" : "1 min",
                        "value" : 58
                     },
                     "end_location" : {
                        "lat" : 43.45758,
                        "lng" : -80.5195739
                     },
                     "html_instructions" : "Turn \u003cb\u003eright\u003c/b\u003e onto \u003cb\u003eIron Horse Trans Canada Trail\u003c/b\u003e",
                     "maneuver" : "turn-right",
                     "polyline" : {
                        "points" : "oaghGdjmjNnBtBFDVLn@Bn@Ab@G"
                     },
                     "start_location" : {
                        "lat" : 43.4589585,
                        "lng" : -80.51891289999999
                     },
                     "travel_mode" : "BICYCLING"
                  },
                  {
                     "distance" : {
                        "text" : "0.1 mi",
                        "value" : 193
                     },
                     "duration" : {
                        "text" : "1 min",
                        "value" : 31
                     },
                     "end_location" : {
                        "lat" : 43.4562196,
                        "lng" : -80.52105019999999
                     },
                     "html_instructions" : "Turn \u003cb\u003eright\u003c/b\u003e onto \u003cb\u003eJohn St W\u003c/b\u003e",
                     "maneuver" : "turn-right",
                     "polyline" : {
                        "points" : "{xfhGhnmjNv@~@hBpBlBtB"
                     },
                     "start_location" : {
                        "lat" : 43.45758,
                        "lng" : -80.5195739
                     },
                     "travel_mode" : "BICYCLING"
                  },
                  {
                     "distance" : {
                        "text" : "0.2 mi",
                        "value" : 369
                     },
                     "duration" : {
                        "text" : "1 min",
                        "value" : 86
                     },
                     "end_location" : {
                        "lat" : 43.45371050000001,
                        "lng" : -80.518275
                     },
                     "html_instructions" : "Turn \u003cb\u003eleft\u003c/b\u003e onto \u003cb\u003eBelmont Ave W\u003c/b\u003e\u003cdiv style=\"font-size:0.9em\"\u003eDestination will be on the right\u003c/div\u003e",
                     "maneuver" : "turn-left",
                     "polyline" : {
                        "points" : "kpfhGpwmjNf@eAzCoGFCDKDKFK|@k@FCDAF@DAfBaArAw@"
                     },
                     "start_location" : {
                        "lat" : 43.4562196,
                        "lng" : -80.52105019999999
                     },
                     "travel_mode" : "BICYCLING"
                  }
               ],
               "traffic_speed_entry" : [],
               "via_waypoint" : []
            }
         ],
         "overview_polyline" : {
            "points" : "wkhhG`cpjNFGBMI]DKnA{@ZIJAMiCGiAEeA@aAFeAPoAUIAASBEHi@_@Wf@c@v@k@~@GIEE?QO[Ua@Q{@K_ABONo@RSBQMc@iAsCCAGCCKAKKKCWF]\\u@Pi@FYJaABQJ[TOj@GRODMG{@dDSPE^M`As@z@_A~@{@jDkC|BiBcAv@i@eBh@dBy@p@|BiBtDqC`BkA\\k@~AgDdD_HJINYn@qAr@wAnBtB^R~A@b@Gv@~@vEfFbEuILOLWdAo@L?lBcArAw@"
         },
         "summary" : "Father David Bauer Dr",
         "warnings" : [
            "Bicycling directions are in beta. Use caution – This route may contain streets that aren't suited for bicycling."
         ],
         "waypoint_order" : [ 0, 1 ]
      }
   ],
   "status" : "OK"
}
```
____
## Rubric

This is part of your first practical lab in Week 3 

1. A working URL properly documented in the MarkDown with a unique origin and destination earns 50%
2. Including one to four additional functioning unique parameters from the API earns 50-70%
3. Having 3 or more functioning unique/novel and well-thought out parameters from the API earns 70-90%
4. Including more than 2 "stops", including links to display PlaceIDs on Google Maps, or other innovative presentations earns 80%-100%. 
