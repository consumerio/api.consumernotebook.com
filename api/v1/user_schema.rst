.. _api-v1-user-schema:

============================
GET /api/v1/user/schema/
============================

Returns the current schema for the Consumer Notebook REST API ``user`` resource. 

Parameters
==========

apikey
    Required for all Consumer Notebook REST API requests. You can also place this in the HTTP_AUTHORIZATION header.

format (optional)
    * json (default)
    * jsonp

Example Request
================

Get::

    curl http://consumernotebook.com/api/v1/users/schema/ -d apikey={apikey} -G
    
Results:
    
.. sourcecode:: javascript

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
            "grids": {
                "blank": false,
                "default": "No default provided.",
                "help_text": "A list of data. Ex: ['abc', 26.73, 8]",
                "nullable": true,
                "readonly": false,
                "type": "list",
                "unique": false
            },
            "lists": {
                "blank": false,
                "default": "No default provided.",
                "help_text": "A list of data. Ex: ['abc', 26.73, 8]",
                "nullable": true,
                "readonly": false,
                "type": "list",
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
            "username": 1
        }
    }