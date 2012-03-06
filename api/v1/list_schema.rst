.. _api-v1-list-schema:

============================
GET /api/v1/lists/schema/
============================

Returns the current schema for the Consumer Notebook REST API ``list`` resource. 

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

    curl http://consumernotebook.com/api/v1/lists/schema/ -d apikey={apikey} -G
    
Results:
    
.. sourcecode:: javascript

    {
        "allowed_detail_http_methods": ["get"],
        "allowed_list_http_methods": ["get"],
        "default_format": "application/json",
        "default_limit": 20,
        "fields": {
            "created": {
                "blank": false,
                "default": "2012-03-06T06:55:53.514757",
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
                "default": "2012-03-06T06:47:21.917746",
                "help_text": "A date & time as a string. Ex: \"2010-11-10T03:07:43\"",
                "nullable": true,
                "readonly": false,
                "type": "datetime",
                "unique": false
            },
            "modified": {
                "blank": false,
                "default": "2012-03-06T06:55:53.514769",
                "help_text": "A date & time as a string. Ex: \"2010-11-10T03:07:43\"",
                "nullable": false,
                "readonly": false,
                "type": "datetime",
                "unique": false
            },
            "owner": {
                "blank": false,
                "default": "No default provided.",
                "help_text": "A single related resource. Can be either a URI or set of nested resource data.",
                "nullable": false,
                "readonly": false,
                "type": "related",
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