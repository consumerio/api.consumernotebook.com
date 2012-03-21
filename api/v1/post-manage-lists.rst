.. _api-v1-post-manage-lists:

===============================
POST /api/v1/post-manage-lists/
===============================

Adds a list. The list is automatically the property of the creating user.

Parameters
==========

access_token
    OAuth2 access token required for all Consumer Notebook REST API requests. 

title
    Name of the list in human readable format.

description (optional)
    A reasonably long description of the purpose of the list.

slug (optional)
    A string made up from characters, numbers, underscores, or hyphens that is unique to the user.
    If a slug is not provided then one will be automatically generated from the title.


Example Request
================

POST::

    curl --dump-header - -H "Content-Type: application/json" -X POST --data '{"title": "test title", "slug":"test-slug", "description":"test description", "access_token":"{access_token}"}' https://consumernotebook.com/api/v1/manage-lists/
    
Results::

    HTTP/1.0 201 CREATED
    Date: Wed, 21 Mar 2012 22:43:32 GMT
    Server: WSGIServer/0.1 Python/2.7.1
    Vary: Cookie
    Content-Type: text/html; charset=utf-8
    Location: https://consumernotebook.com/api/v1/manage-lists/pydanny/test-slug/
    
.. note:: You will have to change the name of 'manage-lists' to 'lists' in order to use this list object for GETs.