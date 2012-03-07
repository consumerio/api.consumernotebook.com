.. _api-v1-grid:

======================
GET /api/v1/grids/{id}
======================

Returns the specified ``grid`` resource.

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

    curl https://consumernotebook.com/api/v1/grids/4f319564bf8bbd000a000000/ -d apikey={apikey} -G
    
Results:    

.. sourcecode:: javascript

    {
        "id": "4f4c6df09acecc000e000002",
        "last_modified_by_user": "2012-02-27T22:18:27.268000",
        "resource_uri": "/api/v1/grids/4f4c6df09acecc000e000002/",
        "slug": "best-wireless-routers",
        "title": "Best Wireless Routers",
        "url": "http://consumernotebook.com/grids/pydanny/best-wireless-routers/",
        "username": "pydanny"
    }