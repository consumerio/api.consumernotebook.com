.. _api-v1-list:

=====================
GET /api/v1/list/{id}
=====================

Returns the list described by the id.

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

    curl https://consumernotebook.com/api/v1/lists/36/ -d access_token={access_token} -G
    
Results:    

.. sourcecode:: javascript

    {
        "created": "2011-12-05T09:37:10.328231",
        "description": "This is a list of every Python programming book I can find. Let me know if you find one not on this list!",
        "id": "36",
        "last_modified_by_user": "2012-02-22T20:49:49.078179",
        "modified": "2012-03-04T20:33:04.033475",
        "owner": {
            "avatar": "/media/avatars/pydanny/resized/80/avatars/pydanny/daniel.greenfeld.jpg",
            "coins": 122,
            "fullname": "Daniel Greenfeld",
            "score": 685,
            "username": "pydanny",
            "waitlisted": false
        },
        "products": [    
            {
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.amazon.com/gp/product/1849515301",
                "id": "4f3c0163ebae26000400002d",
                "image_url": "http://ecx.images-amazon.com/images/I/51o0XqA%2BsLL.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f3c0163ebae26000400002d/",
                "title": "NumPy 1.5 Beginner's Guide"
            },
            {
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.amazon.com/gp/product/1430210478",
                "id": "4f3c0164ebae260004000043",
                "image_url": "http://ecx.images-amazon.com/images/I/41Ry%2BLUNkQL.jpg",
                "price_range": "$20-50",
                "resource_url": "/api/v1/products/4f3c0164ebae260004000043/",
                "title": "Pro Django (Expert's Voice in Web Development)"
            },
            {
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.amazon.com/gp/product/143021936X",
                "id": "4f3c0168ebae260004000070",
                "image_url": "http://ecx.images-amazon.com/images/I/5198kKFjb2L.jpg",
                "price_range": "$20-50",
                "resource_url": "/api/v1/products/4f3c0168ebae260004000070/",
                "title": "The Definitive Guide to Django: Web Development Done Right"
            },
            {
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.amazon.com/gp/product/0321767349",
                "id": "4f3c016bebae2600040000bc",
                "image_url": "http://ecx.images-amazon.com/images/I/518kgosz6XL.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f3c016bebae2600040000bc/",
                "title": "The Python Standard Library by Example (Developer's Library)"
            },
            {
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.amazon.com/gp/product/0672329786",
                "id": "4f3c0176ebae2600040000d8",
                "image_url": "http://ecx.images-amazon.com/images/I/41m7YwHS18L.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f3c0176ebae2600040000d8/",
                "title": "Python Essential Reference (4th Edition)"
            },
            ...
        ],
        "resource_uri": "/api/v1/lists/36/",
        "slug": "complete-list-of-python-programming-books",
        "title": "Complete List of Python Programming Books"
    }