.. _api-v1-put-my-profile:

========================
PUT /api/v1/my-profile/
========================

Parameters
==========

access_token
    OAuth2 access token required for all Consumer Notebook REST API requests.

email
    An email address to use in order to contact you.

fullname
    Your full name. First name, given name, last name, family name, or anything else you want to use.

Example Request
================

Put::

    curl --dump-header - -H "Content-Type: application/json" -X PUT --data '{"fullname": "Daniel A Greenfeld", "access_token":"{access_token}"}' https://consumernotebook.com/api/v1/my-profile/
    
Results::

    HTTP/1.0 204 NO CONTENT
    Date: Wed, 21 Mar 2012 19:38:51 GMT
    Server: WSGIServer/0.1 Python/2.7.1
    Vary: Cookie
    Content-Length: 0
    Content-Type: text/html; charset=utf-8