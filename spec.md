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
		bookPrice : '$402',
		originalPrice : '$459'
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
    { name: "Restaurants", "logo" : ""},
    { name : "Parking", "logo" : ""},
    { name : "Wi-Fi",  "logo" : ""},
    { name : "Fitness Center", "logo" : ""},
    { name: "Outdoor Pool", "logo" :""},
    { name: "Spa", "logo" : ""}
]

// Hotel Object
hotel  =    {
        "id": "55610",
        "name": "THE WESTIN LAKE LAS VEGAS RESORT &amp; SPA",
        "rating": 5,
        "address": "101 MONTELAGO BOULEVARD  HENDERSON",
        "phones": [
            {
              "type": "Unknown",
              "num": "555-0173",
              "countryCode": "1",
              "ext": "123",
              "areaCode": "200"
            }
          ],         
        "descriptions": [
            {
                "Type": "",
                "value": "The luxury hotel radiates a Moroccan atmosphere and comprises a total of 493 rooms spread over 9 floors. Amongst the hotel's facilities count an air-conditioned lobby with a 24-hour reception desk, lift access, a hotel safe, a cloakroom and a currency exchange desk. Further amenities include a newspaper stand, a range of shops, a hairdressing salon, a casino, a kids' club, and free car parking spaces. Dining options include a cozy bar and a pleasing restaurant. Guests may also make use of the public Internet access in addition to the laundry and 24-hour room services. Self and valet parking, secure golf bag storage, concierge-assisted boarding passes, and intra-resort on-demand transportation are also offered."
            }
        ],
        "heroImageUrl": "http://d3mj096p5q0e20.cloudfront.net/ti/HBD/55610/043509a_hb_a_001.jpg",
        "geoCode": {
            "lat" : 36.113,
            "long" : -114.925
        },
        "amenities": [
            {
                "category":"Parking",
                "name":"Long-term parking (surcharge)",                             
                "description" : ""
            }
        ], 
        "images":[
            { "url" : "http://d3mj096p5q0e20.cloudfront.net/fi/HBD/55610/043509a_hb_f_004.jpg", "category" : "room"},
            { "url" : "http://d3mj096p5q0e20.cloudfront.net/fi/HBD/55610/043509a_hb_f_006.jpg", "category" : "hotel"},
            { "url" : "http://d3mj096p5q0e20.cloudfront.net/fi/HBD/55610/043509a_hb_f_007.jpg","category" : "room"},
            { "url" :"http://d3mj096p5q0e20.cloudfront.net/fi/HBD/55610/043509a_hb_w_002.jpg","category" : "hotel"}
        ],
        "areaAttractions":[
            {
                "name":"Las Vegas NV (LAS McCarran Intl)",
                "description":"Las Vegas NV (LAS-McCarran Intl) --3.3 km",
                "category":null
            }
        ],
        "rooms": null,        
        "supportsPostpaidRates": false,
        "supportsPrepaidRates": false       
        
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
    "id": "ad234dw",
    "name": "Pavilion",
    "desc": "Pavilion with 1 bed(s)",
    "roomRate": {
      "fare": {
        "currency": "USD",
        "baseFare": 284.82,
        "fees": [],
        "taxes": [
          {
            "code": null,
            "desc": "TotalTax",
            "amount": 38.12
          }
        ],
        "discount": null, // it is an Array
        "totalFee": 0,
        "totalTax": 38.12,
        "totalDiscount": 0,
        "totalFare": 322.94
      },
      "id":
        "dd01baaa-4f0b-4b01-8fef-17213e21fcbc_13ymjvdineo_1158715_0##MTMxNzExMDsxMjY4MzI1NDsxMDE5NTUxNTsyOzE7MF98VVNHfF8xMjY4MzI1NF98VVNHfF8xLDFffFVTR3xfMV98VVNHfF8=",
      "desc": null,
      "code": "1317110;12683254;10195515;2;1;0",
      "isPrepaid": true,
      "rateType": "Negotiated",
      "depositRequired": false,
      "guaranteeRequired": false,
      "supplierHotelId": "1317110",
      "supplierId": "hbgau0qwow",
      "inclusions": ["Resort Fee for USD 17.90 will be charged by hotel."],
      "additionalCharges": [],
      "refundability": "Unknown",
      "dailyRate": [{
        "date": "2017-01-02",
        "amount": 24.55,
        "discount": 10,
        "taxIncluded": "true"
      }],
      "boardBasis": {
        "code": null,
        "desc": "Continental Breakfast",
        "type": "BedAndBreakfast"
      },
      "cancellationPolicy": {
        "text": "Cancellations or changes made during the applicable cancellation window are subject to a $50 penalty",
        "penaltyRules": [
          {
            "value": 12.34,
            "estimatedValue": 15.5,
            "valueType": "Amount",
            "window": {
              "start": "2017-01-01T01:03",
              "end": "2017-01-25T01:30"
            }
          }
        ]
      },
      "offer":  {
        "title": "Summer Free Nights Bonanza",
        "desc": "Stay for 5 nights and get 2 nights free",
        "discountOffer": 0,
        "percentageDiscountOffer": 0,
        "stayOffer": {
          "stayNights": 5,
          "freeNights": 2
        }
      },
      "policies": [ {
        "type": "Cancellation",
        "text": "Cancellations must be made at least 3 days prior to arrival in order to avoid a full-stay penalty, but not to exceed 3 nights room & tax. For example, a cancellation penalty for a 2-night stay will be 2 nights room and tax. A cancellation penalty for a 5-night stay will be 3 nights room and tax"
      }] 
      
    },
    "adultOccupancy": 1,
    "childOccupancy": 0   
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
        "showMoreRooms" : "Show More Rooms",
	"dailyRates": "Daily Rate"
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
    "more" : "More",
    "foundRightProperty" : "Didn't find the right property?",
    "continueSearch" : "CONTINUE TO SEARCH"
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
- SearchWidget - First time when user lands on Hotel details page ->Modify search button should appear as disabled.
- SearchWidget - If customer click on any of field present on search widgets like "date", "pax selection" etc. the button will start appearing as active.
- Now it will remain active untill customer click on it.
- Room listing - If search is for single room, just mention "Room - RoomName".
- Room listing - Click on "Select" collapse the room so that user can move to other rooms.
- Map - Google zoomIn and zoomOut to show in right most buttom corner
- Show Points of interest in left hand side of map component.

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
