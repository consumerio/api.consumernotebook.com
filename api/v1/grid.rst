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
        "id": "4f319564bf8bbd000a000000",
        "last_modified_by_user": "2012-02-23T15:28:14.892000",
        "resource_uri": "/api/v1/grids/4f319564bf8bbd000a000000/",
        "slug": "must-have-python-programming-books",
        "title": "Must-Have Python Programming Books ",
        "url": "http://consumernotebook.com/grids/pydanny/must-have-python-programming-books/",
        "username": "pydanny"
    }