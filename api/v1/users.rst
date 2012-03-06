.. _api-v1-users:

=====================
GET /api/v1/users/
=====================

Returns the Consumer Notebook users.  This method is can only return up to 20 users at a time.

Parameters
==========

apikey
    Required for all Consumer Notebook REST API requests. You can also place this in the HTTP_AUTHORIZATION header.

format (optional)
    * json (default)
    * jsonp
    
offset (optional)
    Specifies the page of results to retrieve. Defaults to 0.

username (optional)
    This filters by username.

Example Request
================

Get::

    curl https://consumernotebook.com/api/v1/users/ -d apikey={apikey} -d username__startswith=a -G
    
Results:    

.. sourcecode:: javascript

    {
        "meta": {
            "limit": 20,
            "next": "/api/v1/users/?apikey=72c9f72f2ea75b97c0d5b7117344c6a6&limit=20&offset=20",
            "offset": 0,
            "previous": null,
            "total_count": 398
        },
        "objects": [
            {
                "avatar": "https://consumernotebook.s3.amazonaws.com/avatars/adamfast/resized/80/avatars/adamfast/Adamfast.jpg",
                "coins": 10,
                "followers": ["pydanny", "audreyr", "webology"],
                "following": [],
                "fullname": "Adam Fast",
                "grids": [],
                "lists": [{
                    "description": "",
                    "id": 79,
                    "resource_uri": "/api/v1/lists/79/",
                    "title": "My Possessions"
                }],
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
                "grids": [{
                    "description": "test",
                    "id": "4f46137b36593b000c000000",
                    "resource_uri": "/api/v1/grids/4f46137b36593b000c000000/",
                    "title": "test"
                }],
                "lists": [{
                    "description": "",
                    "id": 203,
                    "resource_uri": "/api/v1/lists/203/",
                    "title": "My Wishlist"
                }],
                "resource_uri": "/api/v1/users/94/",
                "score": 5,
                "username": "andrewkornilov",
                "waitlisted": false
            },
            {
                "avatar": "https://consumernotebook.s3.amazonaws.com/avatars/neithere/resized/80/avatars/neithere/neithere.jpg",
                "coins": 0,
                "followers": [],
                "following": [],
                "fullname": "Andy",
                "grids": [{
                    "description": "",
                    "id": "4f48a3e46127f7000d000001",
                    "resource_uri": "/api/v1/grids/4f48a3e46127f7000d000001/",
                    "title": "Smartphones"
                }],
                "lists": [{
                    "description": "",
                    "id": 496,
                    "resource_uri": "/api/v1/lists/496/",
                    "title": "Stuff"
                }],
                "resource_uri": "/api/v1/users/223/",
                "score": 4,
                "username": "neithere",
                "waitlisted": false
            },
            ...
        ]
    }