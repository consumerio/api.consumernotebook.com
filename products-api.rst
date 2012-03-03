============
Products API
============

With the Products API, you can get products that you or other users have bookmarked on Consumer Notebook.

GET /api/v1/products/
======================

.. sourcecode:: javascript

    //  curl --user username:password  https://consumernotebook.com/api/v1/products/
    
    {
        "meta": {
            "limit": 20,
            "next": "/api/v1/products/?limit=20&offset=20",
            "offset": 0,
            "previous": null,
            "total_count": 1115
        },
        "objects": [
            {
                "creator": "pydanny",
                "image_url": "http://ecx.images-amazon.com/images/I/41FgviU3O8L.jpg",
                "pk": "4f3c015febae260004000000",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f3c015febae260004000000/",
                "title": "Stella McCartney womens paisley ash metallic tank top 34",
                "url": "http://go.redirectingat.com?id=26908X855841&xs=1&url=http%3A//www.amazon.com/gp/product/B005SWMIQO"
            },
            {
                "creator": "pydanny",
                "image_url": "http://ecx.images-amazon.com/images/I/31HufOjtq6L.jpg",
                "pk": "4f3c015febae260004000001",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f3c015febae260004000001/",
                "title": "Fujifilm FinePix XP20 Green 14 MP Digital Camera with 5x Optical Zoom and 2.7-Inch LCD",
                "url": "http://go.redirectingat.com?id=26908X855841&xs=1&url=http%3A//www.amazon.com/gp/product/B004JSP8A6"
            },
            ...
        ]
    }            


GET /api/v1/products/schema/
=============================

This command displays the layout of the CN REST API Product object.

.. sourcecode:: javascript

    //  curl --user username:password https://consumernotebook.com/api/v1/products/schema/
    {
        "allowed_detail_http_methods": ["get"],
        "allowed_list_http_methods": ["get"],
        "default_format": "application/json",
        "default_limit": 20,
        "fields": {
            "creator": {
                "blank": false,
                "default": "No default provided.",
                "help_text": "Unicode string data. Ex: \"Hello World\"",
                "nullable": false,
                "readonly": false,
                "type": "string",
                "unique": false
            },
            "image_url": {
                "blank": false,
                "default": "No default provided.",
                "help_text": "Unicode string data. Ex: \"Hello World\"",
                "nullable": false,
                "readonly": false,
                "type": "string",
                "unique": false
            },
            "pk": {
                "blank": false,
                "default": "No default provided.",
                "help_text": "Unicode string data. Ex: \"Hello World\"",
                "nullable": false,
                "readonly": false,
                "type": "string",
                "unique": false
            },
            "price_range": {
                "blank": false,
                "default": "No default provided.",
                "help_text": "Unicode string data. Ex: \"Hello World\"",
                "nullable": false,
                "readonly": false,
                "type": "string",
                "unique": false
            },
            "resource_uri": {
                "blank": false,
                "default": "No default provided.",
                "help_text": "Unicode string data. Ex: \"Hello World\"",
                "nullable": false,
                "readonly": true,
                "type": "string",
                "unique": false
            },
            "title": {
                "blank": false,
                "default": "No default provided.",
                "help_text": "Unicode string data. Ex: \"Hello World\"",
                "nullable": false,
                "readonly": false,
                "type": "string",
                "unique": false
            },
            "url": {
                "blank": false,
                "default": "No default provided.",
                "help_text": "Unicode string data. Ex: \"Hello World\"",
                "nullable": false,
                "readonly": false,
                "type": "string",
                "unique": false
            }
        }
    }