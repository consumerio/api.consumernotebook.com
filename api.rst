============
REST API
============

.. warning:: This is not yet activated on the site. Any and all requests against it will fail until we say so. So there. ;)


Dependencies
============

* An authenticated account.
* A Consumer Notebook API Key

GET https://consumernotebook.com/api/v1/products/
=====================================================

Returns all products in the authenticated user's account, ordered by when they were last modified.

========= ======== ======== ================================================================
Argument  Type     Default  Note
========= ======== ======== ================================================================
api_key   string   Required
username  string   <yours>  Returns products interacted with username. Defaults to your own. 
page      integer  1        A page of 20 Products. Defaults to 1.
from_date datetime n/a      Return only products modified after this time
to_date   datetime n/a      Return only products modified before this time
depth     integer  0        0=basic data;1=adds grids;2=adds lists;3=adds lists/grids
========= ======== ======== ================================================================

Example using depth 0
----------------------

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
    
Examples using depths 1, 2, and 3 forthcoming

GET https://consumernotebook.com/api/v1/lists/
==================================================

Returns all lists in the authenticated user's account.

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

    // GET https://consumernotebook.com/api/v1/lists/?api_key=MYAPIKEY
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

    // GET https://consumernotebook.com/api/v1/lists/?api_key=MYAPIKEY&depth=1
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

GET https://consumernotebook.com/api/v1/grids/
==================================================

Returns all lists in the authenticated user's account.

========= ======== ======= ==========================================================
Argument  Type     Default 
========= ======== ======= ==========================================================
api_key   string   n/a     Required
username  string   <yours> Returns lists belonging to username. Defaults to your own.
page      integer  1       A page of 20 grids. Defaults to 1.
from_date datetime n/a     Return only grids modified after this time
to_date   datetime n/a     Return only grids modified before this time
depth     integer  0       0=titles/description/uri/added; 1=Includes products
========= ======== ======= ==========================================================

Example using depth=0
------------------------

.. sourcecode:: javascript

    // GET https://consumernotebook.com/api/v1/grids/?api_key=MYAPIKEY
    [
        {
            "title": "My favorite comparison", 
            "description": "These things need to be compared"
            "url": "http://consumernotebook.com/grids/pydanny/my-favorite-comparison/",
            "modified": "2012-2-15 11:2:55", 
        },
        ...
    ]

Example using depth=0
------------------------

.. sourcecode:: javascript

    // GET https://consumernotebook.com/api/v1/grids/?api_key=MYAPIKEY&depth=1
    [
        {
            "title": "My favorite comparison", 
            "description": "These things need to be compared"
            "url": "http://consumernotebook.com/grids/pydanny/my-favorite-comparison/",
            "modified": "2012-2-15 11:2:55", 
            "products":
                [
                    TODO
                ]
        },
        ...
    ]