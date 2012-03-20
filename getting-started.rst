===============
Getting Started
===============

Dependencies
============

* An `account on Consumer Notebook`_.
* A `Consumer Notebook API Key`_. 

.. _`account on Consumer Notebook`: http://consumernotebook.com/signup/
.. _`Consumer Notebook API Key`: http://consumernotebook.com/request-api-key/

Authentication
==============

All API calls require an OAuth 2 access token::

    $ curl https://consumernotebook.com/api/v1/lists/ -d access_token={access_token} -G

How this works
--------------

1. Register your OAuth2 consumer application.

2. Obtain an access token.  If your app is a web app, and if it's not entirely AJAX-based, you'll do the following to get it:

    * Your site should have a "Connect" button that links to the Consumer Notebook Connect authorization page::

        https://consumernotebook.com/oauth2/authorize
        ?client_id=YOUR_CLIENT_ID
        &response_type=code
        &redirect_uri=YOUR_REGISTERED_REDIRECT_URI

    * If a user clicks "Allow", they'll get redirected to::

        https://YOUR_REGISTERED_REDIRECT_URI/?code=CODE

    * On your server side, request this::

        https://consumernotebook.com/oauth2/access_token
        ?client_id=YOUR_CLIENT_ID
        &client_secret=YOUR_CLIENT_SECRET
        &grant_type=authorization_code
        &redirect_uri=YOUR_REGISTERED_REDIRECT_URI
        &code=CODE

    * ...and get a JSON response containing an access token::

        { access_token: YOUR_ACCESS_TOKEN }

    * Save the access token in the user's account, so that you can use it until it expires.

3. Make GET or POST requests to the API, passing the access token as a parameter in order to be granted API access::

    access_token=YOUR_ACCESS_TOKEN
    
Filtering
=========

Some of the available REST API resources allow filtering of content. An example is ``username`` on the Users_ resource. Filtering is performed by adding ``username={value}`` to the query string. Example of an exact match::

    curl https://consumernotebook.com/api/v1/users/?username=pydanny&access_token={access_token}

Many REST API filters allow for less specific results by using filter keywords::

    curl https://consumernotebook.com/api/v1/users/?username_startswith=py&access_token={access_token}

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




