.. _api-v1-post-product:

===========================
POST /api/v1/post-product/
===========================

Adds a product, either as a bookmark for existing products or as a new product to the 
Consumer Notebook system.

Parameters
==========

access_token
    OAuth2 access token required for all Consumer Notebook REST API requests.
    
image_url
    Location of an image that represents the product
    
url
    URL of where the product is located on the web.
    
price_range
    The average of the price.
    
title
    Name of the product in human readable format

format (optional)
    * json (default)
    * jsonp


Example Request
================

POST::

    curl --dump-header - -H "Content-Type: application/json" -X POST --data '{"url": "http://www.amazon.com/gp/product/B005ZJ4PT8/", "price_range":"50", "title": "PajamaCity Dinosaur Print Polar Fleece Footed Pajamas", "image_url": "http://ecx.images-amazon.com/images/I/416rcP%2BQqHL.jpg", "access_token":"{access_token}"}' https://consumernotebook.com/api/v1/products/
    
Results::

    HTTP/1.0 201 CREATED
    Date: Wed, 21 Mar 2012 16:12:54 GMT
    Server: WSGIServer/0.1 Python/2.7.1
    Vary: Cookie
    Content-Type: text/html; charset=utf-8
    Location: http://localhost:8000/api/v1/products/4f5122e78db0f8000c000000/