=========
Grids API
=========

GET /api/v1/grids.json
======================

Returns all grids in the specified user's account.

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

    // GET https://consumernotebook.com/api/v1/grids.json?api_key=MYAPIKEY&username=pydanny
    [
        {
            "title": "My favorite comparison", 
            "description": "These things need to be compared"
            "url": "http://consumernotebook.com/grids/pydanny/my-favorite-comparison/",
            "modified": "2012-2-15 11:2:55", 
        },
        ...
    ]

Example using depth=1
------------------------

.. sourcecode:: javascript

    // GET https://consumernotebook.com/api/v1/grids.json?api_key=MYAPIKEY&username=pydanny&depth=1

    [
        {
            "url": "http://consumernotebook.com/grids/pydanny/django-books-1/",
            "title": "Django Books 1", 
            "description": "We built Consumer Notebook with Django as one of the components. ...",
            "modified": "2012-02-16 17:25:41",
            "products": [
                            {"url": "http://consumernotebook.com/pro-django-experts-voice-in-web-development/4f3c0164ebae260004000043/",
                            "title": "Pro Django (Expert's Voice in Web Development)",
                            "image_url": "http://ecx.images-amazon.com/images/I/41Ry%2BLUNkQL.jpg",
                            "modified": "2012-02-26 04:58:32",
                            "external_url": "TODO"},
                        ...
                        ]
        },                                     
        ...
    ]