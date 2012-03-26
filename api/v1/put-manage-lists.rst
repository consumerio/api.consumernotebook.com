.. _api-v1-put-manage-lists:

===============================
PUT /api/v1/post-manage-lists/
===============================

Modifies a list. Only works for lists owned by the user.

.. warning:: This function is in an ALPHA state.

Parameters
==========

access_token
    OAuth2 access token required for all Consumer Notebook REST API requests. 

add_products (optional)
    A comma delineated list of product IDs. Any that are not duplicates are added to the list. TODO - implement

description (optional)
    A reasonably long description of the purpose of the list.

delete_products (optional)
    A comma delineated list of product IDs that are deleted from the list. TODO - implement

slug (optional)
    A string made up from characters, numbers, underscores, or hyphens that is unique to the user.
    If a slug is not provided then one will be automatically generated from the title.

title (optional)
    Name of the list in human readable format.

Example Request
================

POST::

    curl --dump-header - -H "Content-Type: application/json" -X PUT --data '{"title": "test title 1", "slug":"test-slug-1", "description":"test description 1", "access_token":"{{access_token}}"}' https://consumernotebook.com/api/v1/manage-lists/pydanny/test-slug/
    
Results::

    HTTP/1.0 204 NO CONTENT
    Date: Thu, 22 Mar 2012 00:42:03 GMT
    Server: WSGIServer/0.1 Python/2.7.1
    Vary: Cookie
    Content-Length: 0
    Content-Type: text/html; charset=utf-8