.. _api-v1-my-profile:

=======================
GET /api/v1/my-profile/
=======================

Returns your profile.

Parameters
==========

access_token
    OAuth2 access token required for all Consumer Notebook REST API requests.

format (optional)
    * json (default)
    * jsonp
    

Example Request
================

Get::

    curl https://consumernotebook.com/api/v1/my-profile/ -d access_token={access_token} -G
    
Results:    

.. sourcecode:: javascript

    {
        "avatar": "/media/avatars/pydanny/resized/80/avatars/pydanny/daniel.greenfeld.jpg",
        "coins": 122,
        "followers": ["audreyr", "toastythedog", "brantsteen", "eugenemechanism", ...],
        "following": ["kennethlove", "soviet_firstorm", "dmpeters_", "rosalinda-roy", ...],
        "fullname": "Daniel Greenfeld",
        "resource_uri": "/api/v1/my-profile/pydanny/",
        "score": 695,
        "username": "pydanny",
        "waitlisted": false
    }