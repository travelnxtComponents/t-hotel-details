## Scope defination


#### Summary Section

```html
	<hotel-details-heading 
			title="String"
			sub-title = "String"
			rating="4"
			phone=""
			miles=""
			price = [[price]]
			resource = [[resource]] >

	</hotel-details-heading>
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

```
	<hotel-gallary images=[images]></hotel-gallary>


	images = [
			"photo url 1",
			"photo url 2"
	]

```


#### Hotel Details Object

```javascript

hotel  = {
            "id": "55610",
            "name": "THE WESTIN LAKE LAS VEGAS RESORT &amp; SPA",
            "rating": 5,
            "address": "101 MONTELAGO BOULEVARD  HENDERSON",
            "phoneNumber": "702 567 1234",
            "distance": 13.86,
            "description": "The luxury hotel radiates a Moroccan atmosphere and comprises a total of 493 rooms spread over 9 floors. Amongst the hotel's facilities count an air-conditioned lobby with a 24-hour reception desk, lift access, a hotel safe, a cloakroom and a currency exchange desk. Further amenities include a newspaper stand, a range of shops, a hairdressing salon, a casino, a kids' club, and free car parking spaces. Dining options include a cozy bar and a pleasing restaurant. Guests may also make use of the public Internet access in addition to the laundry and 24-hour room services. Self and valet parking, secure golf bag storage, concierge-assisted boarding passes, and intra-resort on-demand transportation are also offered.",
            "descriptions": [
                {
                    "key": "",
                    "value": "The luxury hotel radiates a Moroccan atmosphere and comprises a total of 493 rooms spread over 9 floors. Amongst the hotel's facilities count an air-conditioned lobby with a 24-hour reception desk, lift access, a hotel safe, a cloakroom and a currency exchange desk. Further amenities include a newspaper stand, a range of shops, a hairdressing salon, a casino, a kids' club, and free car parking spaces. Dining options include a cozy bar and a pleasing restaurant. Guests may also make use of the public Internet access in addition to the laundry and 24-hour room services. Self and valet parking, secure golf bag storage, concierge-assisted boarding passes, and intra-resort on-demand transportation are also offered."
                }
            ],
            "heroImageUrl": "http://d3mj096p5q0e20.cloudfront.net/ti/HBD/55610/043509a_hb_a_001.jpg",
            "geoCode": "36.113,-114.925",
            "amenities": [
                {
                    "type": "Hotel",
                    "description": "24h check-in"
                },
                {
                    "type": "Hotel",
                    "description": "24h. Reception"
                },
                {
                    "type": "Room",
                    "description": "Air-conditioned in common areas"
                },
                {
                    "type": "Hotel",
                    "description": "American Express"
                },
                {
                    "type": "Hotel",
                    "description": "Bar-s"
                },
                {
                    "type": "Room",
                    "description": "Bath"
                },
            ],
             "photoUrls": [
                "http://d3mj096p5q0e20.cloudfront.net/fi/HBD/55610/043509a_hb_f_004.jpg",
                "http://d3mj096p5q0e20.cloudfront.net/fi/HBD/55610/043509a_hb_f_006.jpg",
                "http://d3mj096p5q0e20.cloudfront.net/fi/HBD/55610/043509a_hb_f_007.jpg",
                "http://d3mj096p5q0e20.cloudfront.net/fi/HBD/55610/043509a_hb_w_002.jpg",
                "http://d3mj096p5q0e20.cloudfront.net/fi/HBD/55610/043509a_hb_p_003.jpg",
                "http://d3mj096p5q0e20.cloudfront.net/fi/HBD/55610/043509a_hb_r_005.jpg"
            ],
            "pointsOfInterest": [],
            "minFare": {
                "areRatesAvailable": true,
                "fare": {
                    "amount": 165.3,
                    "currency": "USD",
                    "displayAmount": "USD 165.30"
                },
                "equivalentFares": null,
                "equivalents": null
            },
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
                		type: "Agency",
                		"money" : {
	                    	"displayAmount" : "$10",
	                    	"amount" : 10,
	                    	"currency" : "USD"
	                    }
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

            userRating : "3.4",
            userReviewCount : 500
            reviewType : "Excellent"
            
        }
```
#### Room Listing
```html
    <hotel-room-list list=[[rooms]] loading="true|false" >
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
                    		"money" : {
		                    	"displayAmount" : "$10",
		                    	"amount" : 10,
		                    	"currency" : "USD"
		                    }
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

