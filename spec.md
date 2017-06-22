## Scope defination


#### Summary Section

```html
	<t-hotel-details-heading 
			title="String"
			sub-title = "String"
			rating="4"
			phone=""
			miles=""
			price = [[price]]
			resource = [[resource]]>
	</t-hotel-details-heading>
```

```javascript

	price = {
		price : '$402',
		strikeOut : '$459'
		discount : '25%'
	}

	// Default value for resource
	resource = {
		priceLabel = "starting from",
		buttonLabel = "RESERVE"
	}

```

#### Gallary

```html
	<t-gallary 
		   type ="Single | Multiple"
                    images=[images]
                    enable-tiles="true"
		    popup-type = "FullWidth | 50%"
		    >
    </t-gallary>


	images = [
			{ "caption" : "image caption", "url" : "photo url 1", "category" : "room" },
			{ "caption" : "image caption", "url" : "img url 2", "category" : "hotel" }
		]

```




#### Hotel Details Object

```html
    <t-hotel-details
            hotel=[hotel]
            resource = [resource]
            popular-amenities=[popularStaticAmenities]>
    </t-hotel-details>
```

```javascript
//popular amenities - This are static list. For display popular list, need to map these static list with hotel master amenity name.
popularStaticAmenities = [
    "Restaurants",
    "Parking",
    "Wi-Fi",
    "Fitness Center",
    "Outdoor Pool",
    "Spa"
]

// Hotel Object
hotel  = {
            "id": "55610",
            "name": "THE WESTIN LAKE LAS VEGAS RESORT &amp; SPA",
            "rating": 5,
            "address": "101 MONTELAGO BOULEVARD  HENDERSON",
            "phoneNumber": "702 567 1234",
            "distance": 13.86,
            
            "descriptions": [
                {
                    "Type": "",
                    "value": "The luxury hotel radiates a Moroccan atmosphere and comprises a total of 493 rooms spread over 9 floors. Amongst the hotel's facilities count an air-conditioned lobby with a 24-hour reception desk, lift access, a hotel safe, a cloakroom and a currency exchange desk. Further amenities include a newspaper stand, a range of shops, a hairdressing salon, a casino, a kids' club, and free car parking spaces. Dining options include a cozy bar and a pleasing restaurant. Guests may also make use of the public Internet access in addition to the laundry and 24-hour room services. Self and valet parking, secure golf bag storage, concierge-assisted boarding passes, and intra-resort on-demand transportation are also offered."
                }
            ],
            "heroImageUrl": "http://d3mj096p5q0e20.cloudfront.net/ti/HBD/55610/043509a_hb_a_001.jpg",
            "geoCode": {
                "lat" : 36.113
                "long" : -114.925
            },
            "amenities": [
                {
                    "type": "Hotel",
                    "category": "24h check-in",
		    "masterAmentity" : ""
                },
                {
                    "type": "Hotel",
                    "category": "24h. Reception",
		    "masterAmentity" : ""
                },
                {
                    "type": "Room",
                    "category": "Air-conditioned in common areas",
		    "masterAmentity" : ""
                },
                {
                    "type": "Hotel",
                    "category": "American Express",
		    "masterAmentity" : ""
                },
                {
                    "type": "Hotel",
                    "category": "Bar-s",
		    "masterAmentity" : ""
                },
                {
                    "type": "Room",
                    "category": "Bath",
		    "masterAmentity" : ""
                },
            ],
             "photoUrls": [

                { "url" : "http://d3mj096p5q0e20.cloudfront.net/fi/HBD/55610/043509a_hb_f_004.jpg", "category" : "room"},
                { "url" : "http://d3mj096p5q0e20.cloudfront.net/fi/HBD/55610/043509a_hb_f_006.jpg", "category" : "hotel"},
                { "url" : "http://d3mj096p5q0e20.cloudfront.net/fi/HBD/55610/043509a_hb_f_007.jpg","category" : "room"}
                { "url" :"http://d3mj096p5q0e20.cloudfront.net/fi/HBD/55610/043509a_hb_w_002.jpg","category" : "hotel"}
            ],
            "pointsOfInterest": [
                { 
                    "name" : "name",
                    "description": "description"
                }
            ]
            "rooms": null,
            "isCancellable": true,
            "allPassengersInfoRequired": false,
            "isGuaranteeRequired": true,
            "fare": {
                "type": "Published",
                "code": null,
                "isRefundable": false,
                "baseFare" : {
                    	"displayAmount" : "$26.58",
                    	"amount" : 26.58,
                    	"currency" : "USD"
                    },
                "discount":{
                	"displayAmount" : "$10.0",
                	"amount" : 10.00,
                	"currency" : "USD"
                },
                "fees" : [
                	{
                		"type": "Agency",
                        "displayAmount" : "$10",
                        "amount" : 10,
                        "currency" : "USD"
	                    
                	}
                ],
                "totalFee":{
                	"displayAmount" : "$10.00",
                	"amount" : "10",
                	"currency" : "USD"
                },
                "totalTax" : {
                	"displayAmount" : "$5.58",
                	"amount" : 5.58,
                	"currency" : "USD"
                },
                "totalFare" : {
                	"displayAmount" : "$26.58",
                	"amount" : 26.58,
                	"currency" : "USD"
                }
            },
            "isPostPaid": false,
            "isSoldOut": false,
            "isPreferred": false,
            "source": {
                "inventoryId": "55610",
                "id": 111,
                "name": "HotelBeds Test"
            },

            "userRating" : "3.4",
            "userReviewCount" : 500
            "reviewType" : "Excellent"
            
        }
```
#### Room Listing
```html
    <hotel-room-list 
            list=[[rooms]] 
            loading="true|false"
            resource = [[resource]]
            >
    </hotel-room-list>
```


#### Rooms Component Param

```javascript

loading = true; // if value true, then display loading 
//room list object
rooms = 
		[
			{

                "id": "MTAzX18xMzEzMzk5XzEyNTMyMzMwXzkwOTQwNzNfMl8xXzBfXzkwOTE2X18yMS4zNF9ffDF8MTpBOjI1fF9fUGF2aWxpb25QYXZpbGlvbiB3aXRoIDEgYmVkKHMpMXwxfDE6QToyNXw",
                "name": "Pavilion",
                "description": "Pavilion with 1 bed(s)",
                "quantity": 1,
                "isPrepaid": true,
                "guaranteeRequired": false,
                "depositRequired": false,
                "policies": [
                    {
                        "description": "Minimum age for check in is 21 years old with valid id and credit card",
                        "isQuantifiable": false,
                        "window": null,
                        "penalty": null,
                        "type": "Disclaimer"
                    }
                ],
                "fare": {

                    "type": "Published",
                    "code": null,
                    "isRefundable": true,
                    "baseFare" : {
                    	"displayAmount" : "$26.58",
                    	"amount" : 26.58,
                    	"currency" : "USD"
                    },
                    "discount":{
                    	"displayAmount" : "$10.0",
                    	"amount" : 10.00,
                    	"currency" : "USD"
                    },
                    "fees" : [
                    	{
                    		type: "Agency",
                            "displayAmount" : "$10",
                            "amount" : 10,
                            "currency" : "USD"
                    	}
                    ],
                    "totalFee":{
                    	"displayAmount" : "$10.00",
                    	"amount" : "10",
                    	"currency" : "USD"
                    },
                    "totalTax" : {
                    	"displayAmount" : "$5.58",
                    	"amount" : 5.58,
                    	"currency" : "USD"
                    },
                    "totalFare" : {
                    	"displayAmount" : "$26.58",
                    	"amount" : 26.58,
                    	"currency" : "USD"
                    }
                },
                "type": "1313399_12532330_9094073_2_1_0",
                "roomOccupancyTypes": [
                    "|1|1:A:25|"
                ],
                "dailyRates": [
                    {
                        "day": "Tuesday",
                        "amount": 0,
                        "currency": null,
                        "displayAmount": " 0"
                    },
                    {
                        "day": "Wednesday",
                        "amount": 0,
                        "currency": null,
                        "displayAmount": " 0"
                    }
                ],
                "inclusions": [
                    "Resort Fee for USD 17.90 will be charged by hotel."
                ],
                "isPreferred": false,
                "deals": null,
                "source": {
                    "inventoryId": "MTAzX18xMzEzMzk5XzEyNTMyMzMwXzkwOTQwNzNfMl8xXzBfXzkwOTE2X18yMS4zNF9ffDF8MTpBOjI1fF9fUGF2aWxpb25QYXZpbGlvbiB3aXRoIDEgYmVkKHMpMXwxfDE6QToyNXw",
                    "id": 103,
                    "name": "TouricoTGS Test"
                },
                "areExtraTaxesApplicable": false,
                "roomImages":[]
            }
]

```

#### Resource

```json
{
    "room" : {
        "guests" : "Guests",
        "room" : "Room",
        "roomType" : "Room Type",
        "max" : "Max",
        "options" : "Options",
        "price" : "Price",
        "total" : "Total",
        "selected" : "Selected",
        "more" : "more",
        "roomPolicy" : "room Policy",
        "showMoreRooms" : "Show More Rooms"
    },

    "loading" : "Loading..",
    "priceInclusive" : "inclusive of all taxes and fees",
    "description" : "Description",
    "guestReview" : "Guest Review",
    "hotelAmenities" : "Hotel Amenities" ,
    "roomAmenities" : "Room Amenities",
    "hotelPolicies" : "Hotel Policies",
    "pointOfInterest" : "Point of interest",
    "cancellation" : "Cancellation",
    "checkIn" : "Check-in",
    "checkOut" : "Check-out",
    "continueToCheckout" : "CONTINUE TO CHECKOUT",
    "mostPopularAmenities" : "Most Popular Amenities",
    "viewOnMap" : "View on map",
    "more" : "More"
}
```

#### Map Component

```
<t-map 
        enable-nearby=true 
        enable-direction=true 
        center=[[geocode]]
	title = "Hotel Name"
	sub-title = "Address"
        location-name = "Location Name"
	location-details= "Location full address">
</t-map>

/// geocode
geocode = {
    lat : 43.12
    lang : 34.34
}
```

#### Guest Review Summary

```html
    <t-guest-review-summary
            rating = "3.5"
            review-type = "EXCELLENT"
            review-count = "1375">
    </t-guest-review-summary>
```

#### Trust You Review

```html
<t-trustu-review
        trustu-id="trustuid">
</t-trustu-review>

        
```

## Scope
- Component should work across all major browsers - Chrome / Mozilla / Safari / Opera / IE etc.
- Verify all exposed public properties are working independently and with complex combination.
- Verify all exposed methods and events are working.
- Same set of code should work across three views i.e. Desktop/ Tablet and Mobile
- Validations should work for Mandatory fields
- First time when user lands on Hotel details page ->Modify search button should appear as disabled.
- If customer click any of field present on search widgets like "date", "pax selection" etc. the button will start appearing as active.
- Now it will remain active untill customer click on it.

## Steps to Start
- Set Github repository at your end for this project, we will merge them later
- You can use Google/Vaadin's elements (like calendar element and text boxes etc.)

## Performance standard
- Any component if opened via [web page tester](https://www.webpagetest.org/), it should load under 500ms (milli seconds).

## Documents
- Visual designs for components - https://projects.invisionapp.com/share/6E9PJ7R4Q#/screens/234137579
- API access : URL - http://demo.travelnxt.com/dev
- Tavisca Elements - https://github.com/atomelements and https://github.com/travelnxtelements
- Vaadin elements - https://vaadin.com/docs/-/part/elements/elements-getting-started.html
- Google - https://elements.polymer-project.org/browse?package=google-web-components
- Tavisca Web component style Guide - https://drive.google.com/open?id=0B7BT_2nBFNYVR2tscE9pRnVJYmc
