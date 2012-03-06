.. _api-v1-product:

=========================
GET api/v1/products/{id}/
=========================

Returns the product specified by the {id}. The Consumer Notebook {id} is 24 characters long and accepts alphanumeric values.

Parameters
==========

apikey
    Required for all Consumer Notebook REST API requests. You can also place this in the HTTP_AUTHORIZATION header.

format (optional)
    * json (default)
    * jsonp
    * xml
    

Example Request
================

Get::

    curl http://consumernotebook.com/api/v1/products/4f46999dd6771d00c3000000/ -d apikey={apikey} -G
    
Results:
    
.. sourcecode:: javascript

    {
        "creator": "gdorn",
        "image_url": "http://ecx.images-amazon.com/images/I/41iKZfi08bL.jpg",
        "id": "4f46999dd6771d00c3000000",
        "grids": [],
        "lists": [],        
        "price_range": "$1000-2000",
        "resource_uri": "/api/v1/products/4f46999dd6771d00c3000000/",
        "title": "Apple MacBook Air MC965LL/A 13.3-Inch Laptop",
        "url": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.amazon.com/gp/product/B005CWHZP4"
    }