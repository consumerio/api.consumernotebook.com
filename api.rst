============
REST API
============

.. warning:: This is not yet activated on the site. Any and all requests against it will fail until we say so. So there. ;)


Dependencies
============

* An authenticated account.

https://api.consumernotebook.com/v1/products/
=============================================

Returns all products in the user"s account, ordered by when they were last modified.

**Method**: GET

========= ======== ======================================================
Argument  Type     
========= ======== ======================================================
page      integer  A page of 20 Products. Defaults to 1.
from_date datetime Return only products modified after this time
to_date   datetime Return only products modified before this time
========= ======== ======================================================

Example
--------

.. sourcecode:: javascript

    // GET https://api.consumernotebook.com/v1/products/all/
    [
        {
            "title": "Stella McCartney womens paisley ash metallic tank top 34", 
            "purchase_url": "http://amzn.com/B005SWMIQO/",
            "modified": "2012-2-15 11:2:55", 
            "url": "http://consumernotebook.com/lists/stella-mccartney-womens-paisley-ash-metallic-tank-top-34/4f3c015febae260004000000/",
            "image_url": "http://ecx.images-amazon.com/images/I/41FgviU3O8L._SL160_.jpg", 
        },
        ...
    ]

https://api.consumernotebook.com/v1/lists/
==========================================
    

Returns lists from a user"s account.

**Method**: GET

========= ======== ======= ======================================================
Argument  Type     Default 
========= ======== ======= ======================================================
page      integer  1       A page of 20 lists. Defaults to 1.
from_date datetime n/a     Return only lists modified after this time
to_date   datetime n/a     Return only lists modified before this time
depth     integer  0       0=titles/description/uri/added; 1=Includes products
========= ======== ======= ======================================================

Example Depth 0
------------------------

.. sourcecode:: javascript

    // GET https://api.consumernotebook.com/v1/lists/all/
    [
        {
            "title": "My wishlist", 
            "description": "I want all this stuff. And so much more!"
            "url": "http://consumernotebook.com/lists/pydanny/my-wishlist/",
            "modified": "2012-2-15 11:2:55", 
        },
        ...
    ]