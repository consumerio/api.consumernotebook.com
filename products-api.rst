============
Products API
============

With the Products API, you can get products that you or other users have bookmarked on Consumer Notebook.

GET /api/v1/products/
======================

.. sourcecode:: javascript

    //  curl https://consumernotebook.com/api/v1/products/?apikey={apikey}
    
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
                "url": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.amazon.com/gp/product/B005SWMIQO"
            },
            {
                "creator": "pydanny",
                "image_url": "http://ecx.images-amazon.com/images/I/31HufOjtq6L.jpg",
                "pk": "4f3c015febae260004000001",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f3c015febae260004000001/",
                "title": "Fujifilm FinePix XP20 Green 14 MP Digital Camera with 5x Optical Zoom and 2.7-Inch LCD",
                "url": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.amazon.com/gp/product/B004JSP8A6"
            },
            ...
        ]
    }         
    
GET /api/v1/products/<pk>/
===========================

Get a product by it's Consumer Notebook pk.

.. sourcecode:: javascript

    // curl https://consumernotebook.com/api/v1/products/4f3c0161ebae26000400000d/?apikey={apikey}
    {
        "creator": "pydanny",
        "image_url": "http://ecx.images-amazon.com/images/I/51UmKMROcNL.jpg",
        "pk": "4f3c0161ebae26000400000d",
        "price_range": "Coming",
        "resource_uri": "/api/v1/products/4f3c0161ebae26000400000d/",
        "title": "Forbidden Island",
        "url": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.amazon.com/gp/product/B003D7F4YY"
    }
    
Filtering by username
======================

This lists all the products that a person has listed, or compared, or attempted to add to Consumer Notebook.

.. sourcecode:: javascript

    // curl https://consumernotebook.com/api/v1/products/4f3c0161ebae26000400000d/?apikey={apikey}&username=pydanny
    {
        "meta": {
            "limit": 20,
            "next": "/api/v1/products/?username=pydanny&apikey=72c9f72f2ea75b97c0d5b7117344c6a6&limit=20&offset=20",
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

GET /api/v1/products/schema/
=============================

This command displays the layout of the CN REST API Product object.

.. sourcecode:: javascript

    //  curl https://consumernotebook.com/api/v1/products/schema/?apikey={apikey}
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