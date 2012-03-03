============
Users API
============

This API lets you communicate and work with users objects.

GET /api/v1/users/
==================

Get a list of users.

.. sourcecode:: javascript

    // curl --user username:password https://consumernotebook.com/api/v1/users/
    {
        "meta": {
            "limit": 20,
            "next": "/api/v1/users/?limit=20&offset=20",
            "offset": 0,
            "previous": null,
            "total_count": 335
        },
        "objects": [{
            "avatar": "https://consumernotebook.s3.amazonaws.com/avatars/adamfast/resized/80/avatars/adamfast/Adamfast.jpg",
            "coins": 10,
            "followers": ["pydanny", "audreyr", "webology"],
            "following": [],
            "fullname": "Adam Fast",
            "resource_uri": "/api/v1/users/32/",
            "score": 5,
            "username": "adamfast",
            "waitlisted": false
        },
        {
            "avatar": "https://consumernotebook.s3.amazonaws.com/avatars/andrewkornilov/resized/80/avatars/andrewkornilov/andrew.kornilov.jpg",
            "coins": 10,
            "followers": ["pydanny"],
            "following": [],
            "fullname": "Andrew Kornilov",
            "resource_uri": "/api/v1/users/94/",
            "score": 5,
            "username": "andrewkornilov",
            "waitlisted": false
        },
        ...
        }]
    }


GET /api/v1/users/schema/
=========================

Schema representation of Consumer Notebook user objects.

.. sourcecode:: javascript

    // curl --user username:password https://consumernotebook.com/api/v1/users/schema/
    {
        "allowed_detail_http_methods": ["get"],
        "allowed_list_http_methods": ["get"],
        "default_format": "application/json",
        "default_limit": 20,
        "fields": {
            "avatar": {
                "blank": false,
                "default": "No default provided.",
                "help_text": "Unicode string data. Ex: \"Hello World\"",
                "nullable": true,
                "readonly": false,
                "type": "string",
                "unique": false
            },
            "coins": {
                "blank": false,
                "default": 0,
                "help_text": "Integer data. Ex: 2673",
                "nullable": false,
                "readonly": false,
                "type": "integer",
                "unique": false
            },
            "followers": {
                "blank": false,
                "default": "No default provided.",
                "help_text": "A list of data. Ex: ['abc', 26.73, 8]",
                "nullable": true,
                "readonly": false,
                "type": "list",
                "unique": false
            },
            "following": {
                "blank": false,
                "default": "No default provided.",
                "help_text": "A list of data. Ex: ['abc', 26.73, 8]",
                "nullable": true,
                "readonly": false,
                "type": "list",
                "unique": false
            },
            "fullname": {
                "blank": false,
                "default": "No default provided.",
                "help_text": "Unicode string data. Ex: \"Hello World\"",
                "nullable": true,
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
            "score": {
                "blank": false,
                "default": 0,
                "help_text": "Integer data. Ex: 2673",
                "nullable": false,
                "readonly": false,
                "type": "integer",
                "unique": false
            },
            "username": {
                "blank": false,
                "default": "No default provided.",
                "help_text": "Unicode string data. Ex: \"Hello World\"",
                "nullable": true,
                "readonly": false,
                "type": "string",
                "unique": true
            },
            "waitlisted": {
                "blank": false,
                "default": true,
                "help_text": "Boolean data. Ex: True",
                "nullable": false,
                "readonly": false,
                "type": "boolean",
                "unique": false
            }
        },
        "filtering": {
            "username": ["exact"]
        }
    }