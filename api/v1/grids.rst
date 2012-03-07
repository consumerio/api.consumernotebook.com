.. _api-v1-grids:

=====================
GET /api/v1/grids/
=====================

Returns the most recent grids added to Consumer Notebook.  This method is can only return up to 20 grids at a time.

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

    curl https://consumernotebook.com/api/v1/grids/ -d apikey={apikey} -d username=audreyr -G
    
Results:    

.. sourcecode:: javascript

    {
        "meta": {
            "limit": 20,
            "next": "/api/v1/grids/?username=audreyr&apikey={apikey}&limit=20&offset=20",
            "offset": 0,
            "previous": null,
            "total_count": 41
        },
        "objects": [
                "id": "4f4e8aefcac041000d000002",
                "last_modified_by_user": "2012-02-29T15:11:06.182000",
                "resource_uri": "/api/v1/grids/4f4e8aefcac041000d000002/",
                "title": "Apple TV vs. Google TV vs. Roku vs. Boxee",                
                "title": "Apple TV vs. Google TV vs. Roku vs. Boxee",
                "username": "audreyr"
            },
        ],
        ...
    }