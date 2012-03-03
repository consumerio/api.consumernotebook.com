=========
Lists API
=========

GET /api/v1/lists/<list_id>/
============================

.. sourcecode:: javascript

    //  curl --user username:password http://localhost:8000/api/v1/lists/500/
    {
        "created": "2012-02-25T13:24:39.212716",
        "description": "",
        "id": "500",
        "last_modified_by_user": "2012-02-25T11:59:07.083030",
        "modified": "2012-02-26T20:32:19.020097",
        "profile": {
            "avatar": "/media/avatars/pydanny/resized/80/avatars/pydanny/daniel.greenfeld.jpg",
            "coins": 112,
            "fullname": "Daniel Greenfeld",
            "score": 672,
            "username": "pydanny",
            "waitlisted": false
        },
        "resource_uri": "/api/v1/lists/500/",
        "slug": "vita",
        "title": "Vita"        
        "products": [
            {
                "created": "2012-02-25T13:25:00.575560",
                "modified": "2012-02-26T20:31:59.066459",
                "order": 1,
                "product": {
                    "_id": "4f4951ac3ad8f20012000000",
                    "creator": "pydanny",
                    "image_url": "http://ecx.images-amazon.com/images/I/31lvjvwfwxL.jpg",
                    "title": "PlayStation Vita Travel Pouch",
                    "url": "http://go.redirectingat.com?id=26908X855841&xs=1&url=http%3A//www.amazon.com/gp/product/B006PP41Q8"
                },
                "reason": "I want to protect my favorite game device.",
                "resource_uri": ""
            },
            {
                "created": "2012-02-25T13:25:16.295924",
                "modified": "2012-02-26T20:32:02.163021",
                "order": 2,
                "product": {
                    "_id": "4f4951bcdd83af000d000000",
                    "creator": "pydanny",
                    "image_url": "http://ecx.images-amazon.com/images/I/61UdIS4QRTL.jpg",
                    "title": "Rayman Origins: playstation vita: Video Games",
                    "url": "http://go.redirectingat.com?id=26908X855841&xs=1&url=http%3A//www.amazon.com/gp/product/B006WJ6YH6"
                },
                "reason": "Looks like fun!",
                "resource_uri": ""
            },
            ...
        ],
    }


GET /api/v1/lists/schema/
=========================

.. sourcecode:: javascript

    {
        "allowed_detail_http_methods": ["get"],
        "allowed_list_http_methods": ["get"],
        "default_format": "application/json",
        "default_limit": 20,
        "fields": {
            "created": {
                "blank": false,
                "default": "2012-03-02T17:04:42.290540",
                "help_text": "A date & time as a string. Ex: \"2010-11-10T03:07:43\"",
                "nullable": false,
                "readonly": false,
                "type": "datetime",
                "unique": false
            },
            "description": {
                "blank": false,
                "default": "",
                "help_text": "Unicode string data. Ex: \"Hello World\"",
                "nullable": true,
                "readonly": false,
                "type": "string",
                "unique": false
            },
            "id": {
                "blank": false,
                "default": "",
                "help_text": "Unicode string data. Ex: \"Hello World\"",
                "nullable": false,
                "readonly": false,
                "type": "string",
                "unique": true
            },
            "last_modified_by_user": {
                "blank": false,
                "default": "2012-03-02T17:04:28.451838",
                "help_text": "A date & time as a string. Ex: \"2010-11-10T03:07:43\"",
                "nullable": true,
                "readonly": false,
                "type": "datetime",
                "unique": false
            },
            "modified": {
                "blank": false,
                "default": "2012-03-02T17:04:42.290554",
                "help_text": "A date & time as a string. Ex: \"2010-11-10T03:07:43\"",
                "nullable": false,
                "readonly": false,
                "type": "datetime",
                "unique": false
            },
            "products": {
                "blank": false,
                "default": "No default provided.",
                "help_text": "Many related resources. Can be either a list of URIs or list of individually nested resource data.",
                "nullable": false,
                "readonly": false,
                "type": "related",
                "unique": false
            },
            "profile": {
                "blank": false,
                "default": "No default provided.",
                "help_text": "A single related resource. Can be either a URI or set of nested resource data.",
                "nullable": false,
                "readonly": false,
                "type": "related",
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
            "slug": {
                "blank": false,
                "default": "No default provided.",
                "help_text": "Unicode string data. Ex: \"Hello World\"",
                "nullable": false,
                "readonly": false,
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
            }
        }
    }