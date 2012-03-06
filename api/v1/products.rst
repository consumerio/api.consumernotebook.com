.. _api-v1-products:

====================
GET api/v1/products/
====================

Returns the most recent products added to Consumer Notebook.  This method is can only return up to 20 products at a time.

Parameters
==========

apikey
    Required for all Consumer Notebook REST API requests. You can also place this in the HTTP_AUTHORIZATION header.

format (optional)
    * json (default)
    * jsonp
    * xml
    
page (optional)
    Specifies the page of results to retrieve. Defaults to 1.

username (optional)
    This lists all the products that a person has listed, or compared, or attempted to add to Consumer Notebook.

Example Request
================

Get::

    curl https://consumernotebook.com/api/v1/products/ -d apikey={apikey} -d username=pydanny -G
    
Results:    

.. sourcecode:: javascript

    {
        "meta": {
            "limit": 20,
            "next": "/api/v1/products/?apikey=72c9f72f2ea75b97c0d5b7117344c6a6&limit=20&offset=20",
            "offset": 0,
            "previous": null,
            "total_count": 1226
        },
        "objects": [
            {
                "creator": "gdorn",
                "grids": [
                    {
                        "description": "Really good, light laptops.",
                        "id": "4f469943d6771d000e000000",
                        "title": "13\" Ultrabooks"
                    }
                ],
                "id": "4f46999dd6771d00c3000000",
                "image_url": "http://ecx.images-amazon.com/images/I/41iKZfi08bL.jpg",
                "lists": [
                    {
                        "description": "This is a mix of various things I like to call my own.",
                        "id": 6,
                        "title": "My Possessions"
                    }
                ],
                "price_range": "$1000-2000",
                "resource_uri": "/api/v1/products/4f46999dd6771d00c3000000/",
                "title": "Apple MacBook Air MC965LL/A 13.3-Inch Laptop",
                "url": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.amazon.com/gp/product/B005CWHZP4"
            },
            {
                "creator": "pydanny",
                "grids": [{
                    "grid": "",
                    "id": "4f555f83247c21000d000001",
                    "title": "Doctor Who Holiday Specials"
                }],
                "id": "4f555f83247c21000d000000",
                "image_url": "http://ecx.images-amazon.com/images/I/51c5UodsF7L._SX500_.jpg",
                "lists": [{
                    "description": "This is a list of odds and ends I would like to get into my hands. Or at least my Kindle!",
                    "id": 5,
                    "title": "My Wishlist"
                }],
                "price_range": "$0-10",
                "resource_uri": "/api/v1/products/4f555f83247c21000d000000/",
                "title": "Doctor Who: A Christmas Carol - Amazon Instant Video",
                "url": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.amazon.com/gp/product/B004HBVDSQ"
            },
        ...
        ]
    }