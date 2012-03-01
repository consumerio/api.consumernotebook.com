============
Users API
============

GET /api/v1/users.json
=====================================================

Returns information for a specified user's account.

========= ======== ======== ================================================================
Argument  Type     Default  Note
========= ======== ======== ================================================================
api_key   string   Required
username  string   <yours>  Returns data on the specified username. Defaults to your own. 
search    string   
========= ======== ======== ================================================================

Example
-------

.. sourcecode:: javascript

    // GET https://api.consumernotebook.com/api/v1/users.json?api_key=YOURKEYHERE&username=pydanny
    {
        "username": "pydanny", 
        "fullname": "Daniel Greenfeld",
        "avatar": "https://consumernotebook.s3.amazonaws.com/avatars/pydanny/resized/80/avatars/pydanny/daniel.greenfeld.jpg" 
        "badges": ["wisher", "contributor", "beta", "inventory-taker"],
        "joined": "2011-11-12 19:16:55",
        "twitter": "pydanny",
        "facebook": "daniel.greenfeld",
        "points": 673,
        "coins": 112,
        "following": ["audreyr", "knockycode", ...],            
        "followers": ["audreyr", "knockycode", ...],
        "grids": [
            {
                "title": "My favorite comparison", 
                "description": "These things need to be compared"
                "url": "http://consumernotebook.com/grids/pydanny/my-favorite-comparison/",
                "modified": "2012-2-15 11:2:55", 
            },
            ...
        ]
        "lists": [
            {
                "title": "My wishlist", 
                "description": "I want all this stuff. And so much more!"
                "url": "http://consumernotebook.com/lists/pydanny/my-wishlist/",
                "modified": "2012-2-15 11:2:55", 
            },
            ...
        ]
    }
    
POST /api/v1/users/follow/
==========================

Your account will follow the specified username.

========= ======== ======== ===============================
Argument  Type     Default  Note
========= ======== ======== ===============================
api_key   string   Required
username  string   Required Follow another person's account
========= ======== ======== ===============================

Example using depth 0
----------------------

.. parsed-literal::

    // POST https://api.consumernotebook.com/api/v1/users/follow/