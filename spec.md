## Scope defination


#### Summary Section

```html
	<t-hotel-details-heading 
			title="String"
			sub-title = "String"
			rating="4"
			phone=""
			distance=""
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
hotel={
overview : {
  "name": "Westgate Las Vegas Resort & Casino",
  "rating": 4,
  "phone": "",
  "address": "3000 Paradise Road, , Las Vegas 89109",
  "distance":{
    "From":"City Center",
    "amount":3.2
    "unit":"Mile"
  },
  "price":{
		"bookPrice" : "$402",
		"originalPrice" : "$459",
		"discount" : "25%"
	}
},
details  :    {
    "id": "1153848",
    "amenities": [
      { "name": "Pay movies", "description": null, "category": null },
      { "name": "Poolside bar", "description": null, "category": "Bar" },
      { "name": "Private bathroom", "description": null, "category": null },
      { "name": "Elevator/lift", "description": null, "category": null },
      { "name": "Refrigerator", "description": null, "category": null },
      { "name": "Led Tv", "description": null, "category": "Television" },
      { "name": "Porter/bellhop", "description": null, "category": null },
      { "name": "Snack bar/deli", "description": null, "category": "Bar" }
    ],
    "descriptions": [
      {
        "type": "Recreation",
        "value":
          "Westgate Las Vegas Resort & Casino offers a large outdoor pool with brand new cabanas and daybeds, plus an adjacent 25-seat hot tub, a bar, grill, and retail store. The resort also features 6 hard-surface tennis courts (surcharge), 4 of which are lighted for night play. Private tennis lessons are available upon reservation and request. Guests can enjoy the state-of-the-art fitness center that features cardio equipment, free weights, and weight machines, conveniently located at the pool deck. Access to the pool and fitness center is included in the resort fee. The recreational activities listed below are available either on site or nearby; fees may apply."
      },
      {
        "type": "Spa",
        "value":
          "The Spa at Westgate Las Vegas Resort & Casino is currently closed for renovations."
      },
      {
        "type": "General",
        "value":
          "Property Location With a stay at Westgate Las Vegas Resort & Casino in Las Vegas (East of The Strip), you'll be minutes from Las Vegas Convention Center and close to University of Nevada-Las Vegas. This 4-star hotel is within close proximity of Las Vegas Country Club and Fashion Show Mall. Rooms Make yourself at home in one of the 2956 air-conditioned rooms featuring refrigerators and LED televisions. Wired Internet access (surcharge) is available to keep you connected. Private bathrooms with shower/tub combinations feature complimentary toiletries and hair dryers. Conveniences include phones, as well as safes and desks. Amenities Take time to pamper yourself with a visit to the full-service spa. Gambling sorts can try their luck at the casino, while others may prefer outdoor tennis courts or a 24-hour health club. Additional features at this hotel include wireless Internet access (surcharge), concierge services, and gift shops/newsstands. Dining Grab a bite to eat at one of the hotel's 10 restaurants and 2 coffee shops/cafés, or stay in and take advantage of room service (during limited hours). Relax with a refreshing drink from a poolside bar or one of the 5 bars/lounges. Business, Other Amenities Featured amenities include wired Internet access (surcharge), a business center, and limo/town car service. Planning an event in Las Vegas? This hotel has 225,000 square feet (21 square meters) of space consisting of conference space and meeting rooms. Free valet parking is available onsite."
      },
      {
        "type": "Dining",
        "value":
          "Grab a bite to eat at one of the hotel's 10 restaurants and 2 coffee shops/cafés, or stay in and take advantage of room service (during limited hours). Relax with a refreshing drink from a poolside bar or one of the 5 bars/lounges."
      }
    ],
    "heroImageUrl":
      "http://d3mj096p5q0e20.cloudfront.net/fi/HCM/1153848/19558_405_b.jpg",
    "geoCode": { "lat": 36.13603, "long": -115.154709 },
    "images": [
      {
        "url":
          "http://d3mj096p5q0e20.cloudfront.net/fi/HCM/1153848/19558_405_b.jpg",
        "category": "Banquet Hall"
      },
      {
        "url":
          "http://d3mj096p5q0e20.cloudfront.net/fi/HCM/1153848/19558_393_b.jpg",
        "category": "Buffet"
      },
      {
        "url":
          "http://d3mj096p5q0e20.cloudfront.net/fi/HCM/1153848/ee480a2b_b.jpg",
        "category": "Guestroom"
      }
    ],
    "areaAttractions": [
      {
        "name": "Las Vegas NV (LAS McCarran Intl)",
        "description": "Las Vegas NV (LAS-McCarran Intl) --5.6 km",
        "category": null
      }
    ],
    "hotelChain": "Westgate Resorts",
    "policies": [
      {
        "type": "General",
        "text":
          "Know Before You Go The property has connecting/adjoining rooms, which are subject to availability and can be requested by contacting the property using the number on the booking confirmation. Fees The following fees and deposits are charged by the property at time of service, check-in, or check-out. Fee for wireless Internet in public areas: USD 15.99 per night (rates may vary) Fee for wired Internet in public areas: USD 15.99 per stay (rates may vary) Rollaway bed fee: USD 30.00 per night The above list may not be comprehensive. Fees and deposits may not include tax and are subject to change. Mandatory Fees and Taxes You'll be asked to pay the following charges at the property: Resort fee: USD 29.95+tax per accommodation, per night The resort fee includes: Fitness center access Internet access Phone calls Parking Additional inclusions We have included all charges provided to us by the property. However, charges can vary, for example, based on length of stay or the room you book."
      }
    ],
    "fare": null,
    "deal": null,
    "userReview": {
      "rating": "3.5",
      "rype": "Excellent",
      "count": 500
    },
    "checkinCheckoutPolicy": [
      {
        "inTime": "15:0",
        "outTime": "11:0",
        "days": ["Sun", "Mon", "Tue", "Wed", "Thu", "Fri", "Sat"]
      }
    ]
  },
rooms: null,
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
        "id": "8025ec42-019e-494d-b822-801ab926d8ec",
        "name": "Premium",
        "type": "",
        "code": "2023502",
        "desc": "",
        "availableRoomCount": 0,
        "maxOccupancy": 0,
        "adultOccupancy": 2,
        "childOccupancy": 0,
        "smokingIndicator": "Unknown",
        "roomRate": {
          "fare": {
            "currency": "USD",
            "baseFare": 741.83,
            "fees": [],
            "taxes": [{ "code": null, "desc": "TotalTax", "amount": 77.02 }],
            "discounts": null,
            "totalFee": 0.0,
            "totalTax": 77.02,
            "totalDiscount": 0.0,
            "totalFare": 818.85
          },
          "id":
            "9863fd7c-e0ba-4aa6-a69c-20d3a139332c_13ymjvdineo_1153848_0##MTQ4MDU7MjAyMzUwMjsxMjg5MzA7MjsyOzA7MV98VVNHfF8yMDIzNTAyX3xVU0d8XzIsMV98VVNHfF9ffFVTR3xfNQ==",
          "desc": null,
          "code": "14805;2023502;128930;2;2;0;1",
          "isPrepaid": true,
          "rateType": "Negotiated",
          "depositRequired": false,
          "guaranteeRequired": false,
          "supplierHotelId": "14805",
          "inclusions": [],
          "additionalCharges": [
            "Resort Fee for USD 179.70 will be charged by hotel."
          ],
          "refundability": "Unknown",
          "dailyRate": [
            {
              "date": "2017-01-02",
              "amount": 24.55,
              "discount": 10,
              "taxIncluded": "true"
            }
          ],
          "boardBasis": {
            "code": null,
            "desc": "Continental Breakfast",
            "type": "BedAndBreakfast"
          },
          "cancellationPolicy": {
            "text":
              "Cancellations or changes made during the applicable cancellation window are subject to a $50 penalty",
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
          "offer": {
            "title": "Summer Free Nights Bonanza",
            "desc": "Stay for 5 nights and get 2 nights free",
            "discountOffer": 0,
            "percentageDiscountOffer": 0,
            "stayOffer": {
              "stayNights": 5,
              "freeNights": 2
            }
          },
          "policies": [
            {
              "type": "Cancellation",
              "text":
                "Cancellations must be made at least 3 days prior to arrival in order to avoid a full-stay penalty, but not to exceed 3 nights room & tax. For example, a cancellation penalty for a 2-night stay will be 2 nights room and tax. A cancellation penalty for a 5-night stay will be 3 nights room and tax"
            }
          ]
        },
        "recommendationId": "02158680-897f-4111-8a53-664f78b3bd83",
        "bedDetails": [ {
            "type": "King",
            "desc": "King-size bed",
            "count": 1
          }],
        "roomViews": [ "Front view",
            "Sea View"],
        "group": 0
      },
      {
        "id": "41e73bd8-d2d3-4451-b5f4-48942fc3cddb",
        "name": "Premium",
        "type": "",
        "code": "2023502",
        "desc": "",
        "availableRoomCount": 0,
        "maxOccupancy": 0,
        "adultOccupancy": 1,
        "childOccupancy": 0,
        "smokingIndicator": "Unknown",
        "roomRate": {
          "fare": {
            "currency": "USD",
            "baseFare": 741.83,
            "fees": [],
            "taxes": [{ "code": null, "desc": "TotalTax", "amount": 77.02 }],
            "discounts": null,
            "totalFee": 0.0,
            "totalTax": 77.02,
            "totalDiscount": 0.0,
            "totalFare": 818.85
          },
          "id":
            "9863fd7c-e0ba-4aa6-a69c-20d3a139332c_13ymjvdineo_1153848_0##MTQ4MDU7MjAyMzUwMjsxMjg5MzA7MjsxOzBffFVTR3xfMjAyMzUwMl98VVNHfF8xLDFffFVTR3xfX3xVU0d8XzU=",
          "desc": null,
          "code": "14805;2023502;128930;2;1;0",
          "isPrepaid": true,
          "rateType": "Negotiated",
          "depositRequired": false,
          "guaranteeRequired": false,
          "supplierHotelId": "14805",
          "inclusions": [],
          "additionalCharges": [
            "Resort Fee for USD 179.70 will be charged by hotel."
          ],
          "refundability": "Unknown",
          "dailyRate": [
            {
              "date": "2017-01-02",
              "amount": 24.55,
              "discount": 10,
              "taxIncluded": "true"
            }
          ],
          "boardBasis": {
            "code": null,
            "desc": "Continental Breakfast",
            "type": "BedAndBreakfast"
          },
          "cancellationPolicy": null,
          "offer": null,
          "policies": []
        },
        "recommendationId": "02158680-897f-4111-8a53-664f78b3bd83",
        "bedDetails": null,
        "roomViews": [],
        "group": 1
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
