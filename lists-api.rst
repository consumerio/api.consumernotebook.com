=========
Lists API
=========

GET /api/v1/lists/
==================

.. sourcecode:: javascript

    {
        "meta": {
            "limit": 20,
            "next": "/api/v1/lists/?limit=20&offset=20",
            "offset": 0,
            "previous": null,
            "total_count": 218
        },
        "objects": [{
            "created": "2012-02-27T15:44:27.145068",
            "description": "",
            "id": "509",
            "last_modified_by_user": "2012-02-27T12:53:12.956102",
            "modified": "2012-02-27T15:44:27.150332",
            "products": [{
                "created": "2012-02-27T15:44:27.451160",
                "modified": "2012-02-27T15:44:27.494423",
                "order": 0,
                "product": {
                    "_id": "4f4c155b02be66000e000002",
                    "creator": "audreyr",
                    "image_url": "http://ecx.images-amazon.com/images/I/31O2AS6XdAL.jpg",
                    "title": "100% Pure Unrefined Organic Raw Shea Butter (1 Pound)",
                    "url": "http://go.redirectingat.com?id=26908X855841&xs=1&url=http%3A//www.amazon.com/gp/product/B004YBW5T0"
                },
                "reason": "Real butter is best!",
                "resource_uri": ""
            }],
            "profile": {
                "avatar": "https://consumernotebook.s3.amazonaws.com/avatars/audreyr/resized/80/avatars/audreyr/audreyr.jpg",
                "coins": 149,
                "fullname": "Audrey M. Roy",
                "score": 978,
                "username": "audreyr",
                "waitlisted": false
            },
            "resource_uri": "/api/v1/lists/509/",
            "slug": "raw-ingredients",
            "title": "Raw Ingredients"
        },
        {
            "created": "2012-02-27T14:04:27.531537",
            "description": "I went to the Beverly Hills Wine Festival on February 26. Here are the wines I really liked.",
            "id": "508",
            "last_modified_by_user": "2012-02-27T14:23:37.782213",
            "modified": "2012-02-27T14:23:37.801999",
            "products": [{
                "created": "2012-02-27T14:04:27.870567",
                "modified": "2012-02-27T14:28:13.192584",
                "order": 0,
                "product": {
                    "_id": "4f4bfdeb776e5e000e000001",
                    "creator": "audreyr",
                    "image_url": "http://blueplatewines.com/wp-content/uploads/2011/03/bottle.png",
                    "title": "2010 Blue Plate Clarksburg Chenin Blanc",
                    "url": "http://go.redirectingat.com?id=26908X855841&xs=1&url=http%3A//blueplatewines.com/"
                },
                "reason": "One of those complex multi-stage flavor wines, with hints of papaya.",
                "resource_uri": ""
            }],
            "profile": {
                "avatar": "https://consumernotebook.s3.amazonaws.com/avatars/audreyr/resized/80/avatars/audreyr/audreyr.jpg",
                "coins": 149,
                "fullname": "Audrey M. Roy",
                "score": 978,
                "username": "audreyr",
                "waitlisted": false
            },
            "resource_uri": "/api/v1/lists/508/",
            "slug": "wines-i-liked-at-the-beverly-hills-wine-festival",
            "title": "Wines I Liked at the Beverly Hills Wine Festival"
        },
        ...
    }]

GET /api/v1/lists/<list_id>/
============================

.. sourcecode:: javascript

    //  curl --user username:password http://consumernotebook.com/api/v1/lists/500/
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

    //  curl --user username:password http://consumernotebook.com/api/v1/lists/schema/
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