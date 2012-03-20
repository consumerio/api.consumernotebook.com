.. _api-v1-schema:

============================
GET /api/v1/products/schema/
============================

Returns the current schema for the Consumer Notebook REST API ``product`` resource. 

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

    curl http://consumernotebook.com/api/v1/products/schema/ -d access_token={access_token} -G
    
Results:
    
.. sourcecode:: javascript

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
            "grids": {
                "blank": false,
                "default": "No default provided.",
                "help_text": "A list of data. Ex: ['abc', 26.73, 8]",
                "nullable": true,
                "readonly": false,
                "type": "list",
                "unique": false
            },
            "id": {
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
            "lists": {
                "blank": false,
                "default": "No default provided.",
                "help_text": "A list of data. Ex: ['abc', 26.73, 8]",
                "nullable": true,
                "readonly": false,
                "type": "list",
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