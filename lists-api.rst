=========
Lists API
=========

GET /api/v1/lists.json
======================

Returns all lists in the specified user's account.

========= ======== ======= ===========================================================
Argument  Type     Default 
========= ======== ======= ===========================================================
api_key   string   n/a     Required
username  string   <yours> Returns grids belonging to username. Defaults to your own. 
page      integer  1       A page of 20 lists. Defaults to 1.
from_date datetime n/a     Return only lists modified after this time
to_date   datetime n/a     Return only lists modified before this time
depth     integer  0       0=titles/description/uri/added; 1=Includes products
========= ======== ======= ===========================================================

Example using depth=0
------------------------

.. sourcecode:: javascript

    // GET https://consumernotebook.com/api/v1/lists.json?api_key=MYAPIKEY
    [
        {
            "title": "My wishlist", 
            "description": "I want all this stuff. And so much more!"
            "url": "http://consumernotebook.com/lists/pydanny/my-wishlist/",
            "modified": "2012-2-15 11:2:55", 
        },
        ...
    ]

Example using depth=1
------------------------

.. sourcecode:: javascript

    // GET https://consumernotebook.com/api/v1/lists.json?api_key=MYAPIKEY&depth=1
    [
        {
            "title": "Carpal Tunnel / RSI Relief Products", 
            "description": "A list of useful products for people with carpal tunnel/RSI."
            "url": "http://consumernotebook.com/lists/pydanny/my-wishlist/",
            "modified": "2012-2-15 11:20:55", 
            "products": [
                {
                    "title": "The Hand Reflexology Massager by Hammacher Schlemmer",
                    "comment": "You put your hand in the device, press a button, and let it massage your hand for 15 minutes.",
                    "modified": "2012-2-15 11:20:55",
                    "url": "http://consumernotebook.com/the-hand-reflexology-massager-by-hammacher-schlemmer/4f41fc06758920000a000004/",
                    "external_url": "http://go.redirectingat.com/?id=26908X855841&xs=1&url=http%3A//www.hammacher.com/Product/Default.aspx%3Fsku%3D81569%26refsku%3D76527%26xsp%3D3%26promo%3Dxsells"
                },
                {
                    "title": "The Hand Fitness Trainer by Hammacher Schlemmer",
                    "comment": "Helps you exercise those little, hard-to-exercise hand muscles.",
                    "modified": "2012-2-15 09:21:23"
                    "url": "http://consumernotebook.com/the-hand-fitness-trainer-by-hammacher-schlemmer/4f41fc2ae7615d000b000004/",
                    "external_url": "http://go.redirectingat.com/?id=26908X855841&xs=1&url=http%3A//www.hammacher.com/Product/Default.aspx%3Fsku%3D76527%26promo%3DSports-Leisure-Art-Music%26catid%3D227"
                },
                ...
            ]
        },
        ...
    ]
    
POST /api/v1/lists/create/
=========================

TODO

POST /api/v1/lists/delete/
=========================

TODO