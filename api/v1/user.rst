.. _api-v1-user:

======================
GET /api/v1/users/{id}
======================

Returns the Consumer Notebook user specified by the ``{id}``.

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

    curl https://consumernotebook.com/api/v1/users/4/ -d apikey={apikey} -G
    
Results:    

.. sourcecode:: javascript

    {
        "avatar": "/media/avatars/pydanny/resized/80/avatars/pydanny/daniel.greenfeld.jpg",
        "coins": 122,
        "followers": ["audreyr", "toastythedog", "brantsteen", "eugenemechanism", "webology", ...],
        "following": ["kennethlove", "soviet_firstorm", "rosalinda-roy", "kennethreitz" ,..],
        "fullname": "Daniel Greenfeld",
        "grids": [
            {
                "description": "I want to have a collection of the most stylish and crazy pajamas on the planet. Then I can say that I've won!",
                "id": "4f3088db39006c000a000000",
                "resource_uri": "/api/v1/grids/4f3088db39006c000a000000/",
                "title": "Wacky Pajamas"
            },        
            {
                "description": "We built Consumer Notebook with Django as one of the components. Here are a set of references that are available for study.",
                "id": "4f2ff7882570ad000b000000",
                "resource_uri": "/api/v1/grids/4f2ff7882570ad000b000000/",
                "title": "Django Books 1"
            },
            {
                "description": "These are martial arts films about technique, style, and ability.",
                "id": "4f300cfb5b5915000b000000",
                "resource_uri": "/api/v1/grids/4f300cfb5b5915000b000000/",
                "title": "Technical Martial Arts Movies 1"
            },
        ],
        "lists": [
            {
                "description": "It can be hard to buy gifts for an active, retired mom. These are nice, affordable gifts any mother would love.",
                "id": 523,
                "resource_uri": "/api/v1/lists/523/",
                "title": "Gifts to give your retired mom"
            },
            {
                "description": "Help me fill this out. Send me recommendations to my twitter account as pydanny.",
                "id": 503,
                "resource_uri": "/api/v1/lists/503/",
                "title": "Complete List of Python Editors"
            },
            ...
        ],
        "resource_uri": "/api/v1/users/4/",
        "score": 685,
        "username": "pydanny",
        "waitlisted": false
    }