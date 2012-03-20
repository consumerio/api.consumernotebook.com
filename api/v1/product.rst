.. _api-v1-product:

===========================
GET /api/v1/products/{id}/
===========================

Returns the product specified by the {id}. The Consumer Notebook {id} is 24 characters long and accepts alphanumeric values.

Parameters
==========

access_token
    Oauth2 access token required for all Consumer Notebook REST API requests.

format (optional)
    * json (default)
    * jsonp
    

Example Request
================

Get::

    curl http://consumernotebook.com/api/v1/products/4f555f83247c21000d000000/ -d access_token={access_token} -G
    
Results:
    
.. sourcecode:: javascript

    {
        "creator": "gdorn",
        "grids": [
            {
                "description": "Really good, light laptops.",
                "id": "4f469943d6771d000e000000",
                "resource_uri": "/api/v1/grids/4f469943d6771d000e000000/",
                "title": "13\" Ultrabooks",
            }
        ],
        "id": "4f46999dd6771d00c3000000",
        "image_url": "http://ecx.images-amazon.com/images/I/41iKZfi08bL.jpg",
        "lists": [
            {
                "description": "This is a mix of various things I like to call my own.",
                "id": 6,
                "resource_uri": "/api/v1/lists/6/",
                "title": "My Possessions"
            }
        ],
        "price_range": "$1000-2000",
        "resource_uri": "/api/v1/products/4f46999dd6771d00c3000000/",
        "title": "Apple MacBook Air MC965LL/A 13.3-Inch Laptop",
        "url": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.amazon.com/gp/product/B005CWHZP4"
    }