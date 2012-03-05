===============
Getting Started
===============

Dependencies
============

* An authenticated account.
* A Consumer Notebook API Key. If you don't have one, `please request an API Key`_. You'll need to have created an account, but you can play with the API even while on the waitlist.

.. _`please request an API Key`: http://consumernotebook.com/request-api-key/

Authentication
==============

All API calls require an API key::

    $ curl https://consumernotebook.com/api/v1/lists/ -d apikey={apikey} -G
    
You can also pass in the API key as an HTTP header::

    $ TODO show this in the HTTP_AUTHORIZATION header

Filtering
=========

Some of the available REST API resources allow filtering of content. An example is ``username`` on the Users_ resource. Filtering is performed by adding ``username={value}`` to the query string. Example of an exact match::

    curl https://consumernotebook.com/api/v1/users/?username=pydanny&apikey={apikey}

Many REST API filters allow for less specific results by using filter keywords::

    curl https://consumernotebook.com/api/v1/users/?username_startswith=py&apikey={apikey}

The available filterable fields and keywords are detailed in the REST API documentation for each resource.

.. _Users: http://api.consumernotebook.com/en/latest/users-api.html

API Schema
==========

To confirm that you have the most recent documentation, it is suggested that
you validate your code against the following:

.. sourcecode:: javascript

    // curl https://consumernotebok.com/api/v1/
    {
        "lists": {
            "list_endpoint": "/api/v1/lists/", 
            "schema": "/api/v1/lists/schema/"
        }, 
        "products": {
            "list_endpoint": "/api/v1/products/",
            "schema": "/api/v1/products/schema/"
        }, 
        "users": {
            "list_endpoint": "/api/v1/users/",
            "schema": "/api/v1/users/schema/"
        }
    }

.. _python-cn-client: https://github.com/consumernotebook/python-cn-client
.. _`Daniel Greenfeld`: http://pydanny.com




