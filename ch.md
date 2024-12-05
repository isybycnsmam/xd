Read our [blog post](https://medium.com/guestline-labs/hints-for-our-interview-process-and-code-test-ae647325f400) that gives good insight into what we value in the code.

# The Challenge:  

**Create a program to preview hotel room availability and reservations. 
The application should read from files containing hotel data and booking data, 
then allow a user to check room availability for a specified hotel, date range, and room type.**

**Example command:** myapp --hotels hotels.json --bookings bookings.json 

**Example hotels.json**
```json
[
    {
        "id": "H1",
        "name": "Hotel California",
        "roomTypes": [
            {
                "code": "SGL",
                "description": "Single Room",
                "amenities": [
                    "WiFi",
                    "TV"
                ],
                "features": [
                    "Non-smoking"
                ]
            },
            {
                "code": "DBL",
                "description": "Double Room",
                "amenities": [
                    "WiFi",
                    "TV",
                    "Minibar"
                ],
                "features": [
                    "Non-smoking",
                    "Sea View"
                ]
            }
        ],
        "rooms": [
            {
                "roomType": "SGL",
                "roomId": "101"
            },
            {
                "roomType": "SGL",
                "roomId": "102"
            },
            {
                "roomType": "DBL",
                "roomId": "201"
            },
            {
                "roomType": "DBL",
                "roomId": "202"
            }
        ]
    }
]
```

<br>

**Example bookings.json**
```json
[
    {
        "hotelId": "H1",
        "arrival": "20240901",
        "departure": "20240903",
        "roomType": "DBL",
        "roomRate": "Prepaid"
    },
    {
        "hotelId": "H1",
        "arrival": "20240902",
        "departure": "20240905",
        "roomType": "SGL",
        "roomRate": "Standard"
    }
]
```

<br>

Example console input: 

Availability(H1, 20240901, SGL) 

Availability(H1, 20240901-20240903, DBL) 

Output:
 the program should give the availability
 count for the specified room type and date range. 


Note:
hotels sometimes accept over bookings so the value can be negative to indicate this.  

The program should exit when a blank line is entered.  



## General notes: 

Try to code the challenge as you would approach any typical work task; 
We are not looking for you to show knowledge of frameworks or unusual programming language features.
Most importantly, keep it simple.
Computational complexity is not going to be a priority when the solution is evaluated. 

For everything that has not been specified assume that we had a
simple solution in mind. When in doubt feel free to ask questions. 

Please include a link to the source on a public repository (e.g. github)
which includes instructions on how to build and run it and send it back to me.  

There are no timescales here we appreciate you taking the time out to complete the activity. 

If you use a language model (LLM) to complete this code test, please share the prompts you used.
Be aware that we will ask detailed questions about both the solution and the prompts you submitted. 

We're really excited to see what you can do! 


Please do let us know you've received our test by replying to this email. Good Luck! 