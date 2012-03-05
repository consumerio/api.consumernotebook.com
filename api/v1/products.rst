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

    // curl https://consumernotebook.com/api/v1/products/?apikey={apikey}&username=pydanny

    {
        "meta": {
            "limit": 20,
            "next": "/api/v1/products/?username=pydanny&apikey={apikey}&limit=20&offset=20",
            "offset": 0,
            "previous": null,
            "total_count": 266
        },
        "objects": [
            {
                "creator": "pydanny",
                "image_url": "http://ecx.images-amazon.com/images/I/416rcP%2BQqHL.jpg",
                "pk": "4f5122e78db0f8000c000000",
                "price_range": "$20-50",
                "resource_uri": "/api/v1/products/4f5122e78db0f8000c000000/",
                "title": "PajamaCity Dinosaur Print Polar Fleece Footed Pajamas with Drop Seat for Teens and Adults",
                "url": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.amazon.com/gp/product/B005ZJ4PT8"
            },
            {
                "creator": "pydanny",
                "image_url": "http://ecx.images-amazon.com/images/I/51xd5JLUbDL.jpg",
                "pk": "4f5054f57eb9f6000c000000",
                "price_range": "$20-50",
                "resource_uri": "/api/v1/products/4f5054f57eb9f6000c000000/",
                "title": "The 7 Powers of Questions: Secrets to Successful Communication in Life and at Work by Dorothy Leeds",
                "url": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.amazon.com/gp/product/0399526145"
            },
        ...
        ]
    }