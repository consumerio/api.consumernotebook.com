============
Advanced API
============

.. warning:: This is not yet activated on the site. Any and all requests against it will fail until we say so. So there. ;)

Dependencies
============

* An authenticated account.

https://api.consumernotebook.com/v1/products/all
=================================================

Returns all products in the user"s account.

**Method**: GET

========= ======== ======================================================
Argument  Type     
========= ======== ======================================================
page      integer  A page of 20 Products.
from_date datetime Return only products added after this time
to_date   datetime Return only products created before this time
========= ======== ======================================================

Example
--------

.. sourcecode:: javascript

    [
        {
            "title": "Stella McCartney womens paisley ash metallic tank top 34", 
            "url": "http://amzn.com/B005SWMIQO/",
            "added": "2012-2-15 11:2:55", 
            "slug": "stella-mccartney-womens-paisley-ash-metallic-tank-top-34",
            "image_url": "http://ecx.images-amazon.com/images/I/41FgviU3O8L._SL160_.jpg", 
            "pk": "4f3c015febae260004000000",
            "adder": "audreyr",
        }
    ]

    

