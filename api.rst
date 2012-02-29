============
REST API
============

.. warning:: This is not yet activated on the site. Any and all requests against it will fail until we say so. So there. ;)


Dependencies
============

* An authenticated account.
* A Consumer Notebook API Key

GET https://consumernotebook.com/api/v1/products/all/
=====================================================

Returns all products in the authenticated user's account, ordered by when they were last modified.

========= ======== ======================================================
Argument  Type     
========= ======== ======================================================
api_key   string   Required
page      integer  A page of 20 Products. Defaults to 1.
from_date datetime Return only products modified after this time
to_date   datetime Return only products modified before this time
========= ======== ======================================================

Example
--------

.. sourcecode:: javascript

    // GET https://api.consumernotebook.com/api/v1/products/all/?api_key=MYAPIKEY
    [
        {
            "title": "Stella McCartney womens paisley ash metallic tank top 34", 
            "url": "http://consumernotebook.com/lists/stella-mccartney-womens-paisley-ash-metallic-tank-top-34/4f3c015febae260004000000/",
            "image_url": "http://ecx.images-amazon.com/images/I/41FgviU3O8L._SL160_.jpg", 
            "external_url": "http://amzn.com/B005SWMIQO/",
            "modified": "2012-2-15 11:2:55"
        },
        ...
    ]

GET https://consumernotebook.com/api/v1/lists/all/
==================================================

Returns all lists in the authenticated user's account.

========= ======== ======= ======================================================
Argument  Type     Default 
========= ======== ======= ======================================================
api_key   string   n/a     Required
page      integer  1       A page of 20 lists. Defaults to 1.
from_date datetime n/a     Return only lists modified after this time
to_date   datetime n/a     Return only lists modified before this time
depth     integer  0       0=titles/description/uri/added; 1=Includes products
========= ======== ======= ======================================================

Example using depth=0
------------------------

.. sourcecode:: javascript

    // GET https://consumernotebook.com/api/v1/lists/all/?api_key=MYAPIKEY
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

    // GET https://consumernotebook.com/api/v1/lists/all/??api_key=MYAPIKEY&depth=1
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
