==========
API Wide
==========

To confirm that you have the most recent documentation, it is suggested that
you validate your code against the following:

.. sourcecode:: json

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