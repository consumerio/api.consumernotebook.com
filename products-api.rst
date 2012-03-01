============
Products API
============

GET https://consumernotebook.com/api/v1/products/
=====================================================

Returns all products in the specified user's account, ordered by when they were last modified.

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
