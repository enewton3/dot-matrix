# dot-matrix Project Overview

## Project Name

Dot Matrix
Deployed Link :  _______________


## Project Description

This application uses the TransitLand v1 API (will upgrade to v2 when released) to display nearby transit stops that can be filtered based on user input.

Stretch goal - desktop version

Stretch goal - add departure times to nearby stop information.

Stretch goal - save user information and preferences for later use.

## API and Data Sample
ENDPOINTS BEING USED: 
https://transit.land/api/v1/routes?operated_by=o-drt-mbta&per_page=500 (gets all routes operated by a specific operator, sticking with MBTA for now. Will upgrade later)

/api/v1/stops?lon=-121.977772198&lat=37.413530093&r=100 (finds stops within a certain radius(r) of a lat and long)

/api/v1/stops?served_by=r-drt3p-blueline (searches for stops served by a line ID)

```json
{
    "stops": [
        {
            "geometry": {
                "type": "Point",
                "coordinates": [
                    -71.062037,
                    42.361365
                ]
            },
            "onestop_id": "s-drt2yzwhyd-bowdoin<70038",
            "created_at": "2016-05-05T18:06:48.090Z",
            "updated_at": "2020-08-03T20:34:16.680Z",
            "tags": {
                "zone_id": "RapidTransit",
                "stop_url": "https://www.mbta.com/stops/place-bomnl",
                "stop_desc": "Bowdoin - Blue Line - Wonderland",
                "osm_way_id": "387747206",
                "wheelchair_boarding": "0"
            },
            "created_or_updated_in_changeset_id": 15215,
            "name": "Bowdoin",
            "timezone": "America/New_York",
            "osm_way_id": 387747206,
            "served_by_vehicle_types": [
                "metro"
            ],
            "parent_stop_onestop_id": "s-drt2yzwhyd-bowdoin",
            "wheelchair_boarding": false,
            "geometry_reversegeo": null,
            "geometry_centroid": {
                "type": "Point",
                "coordinates": [
                    -71.062037,
                    42.361365
                ]
            },
            "operators_serving_stop": [
                {
                    "operator_name": "Massachusetts Bay Transportation Authority",
                    "operator_onestop_id": "o-drt-mbta"
                }
            ],
            "routes_serving_stop": [
                {
                    "operator_name": "Massachusetts Bay Transportation Authority",
                    "operator_onestop_id": "o-drt-mbta",
                    "route_name": "Blue Line",
                    "route_onestop_id": "r-drt3p-blueline"
                }
            ]
        },

```

## Wireframes

![homepage](/assets/Homepage.png?raw=true "Home Page")
![page 2](/assets/page2.png?raw=true "Page 2" )


## MVP/PostMVP

#### MVP 

- Can pull user location using geolocation object and getCurrentPosition()
- Allows user to filter viewed modes of travel
- Displays nearby transit stops 
- user can search for transit stop if they don't want to give location


#### PostMVP  

- Displays time until next departure for each stop
- Desktop version
- Use local storage to save user preferences

## Project Schedule

|  Day | Deliverable | Status
|---|---| ---|
|Nov 9| Prompt / Wireframes / Priority Matrix / Timeframes | Incomplete
|Nov 10| Project Approval | Incomplete
|Nov 12| Core Application Structure (HTML, CSS, etc.) Begin on JS | Incomplete
|Nov 13| Pseudocode / actual code | Incomplete
|Nov 16| MVP | Incomplete
|Nov 17| Presentations | Incomplete

## Priority Matrix

Include a full list of features that have been prioritized based on the `Time and Importance` Matrix.  Link this image in a similar manner to your wireframes

## Timeframes

| Component | Priority | Estimated Time | Time Invested | Actual Time |
| --- | :---: |  :---: | :---: | :---: |
| Finding/figuring Out APIs | H | 1hrs| 3hrs | 3hrs |
| Build out Base HTML | H | 2hrs| 0hrs | 0hrs |
| Search and Filter HTML inputs | 1hr | 0hrs | 0hrs |
| Build out CSS Styling | H | 3hrs| 0hrs | 0hrs |
| Build out JS functions to pull data | H | 4hrs| 0hrs | 0hrs |
| Build out JS functions to filter data | H | 3hrs| 0hrs | 0hrs |
| Build out JS to pull location data | H | 3hrs| 0hrs | 0hrs |
| Build out JS functions to dynamically display nearby stops | H | 3hrs| 0hrs | 0hrs |
| Use local storage to add save preference functionality | M | 2hrs | 0hrs | 0hrs|
| Figure out getting departure data | M | 2hrs | 0hrs | 0hrs |
| Total | H | 6hrs| 5hrs | 5hrs |

## Code Snippet

Use this section to include a brief code snippet of functionality that you are proud of and a brief description.  

```
function reverse(string) {
	// here is the code to reverse a string of text
}
```

## Change Log
 Use this section to document what changes were made and the reasoning behind those changes.  
