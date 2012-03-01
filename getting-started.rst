===============
Getting Started
===============

Dependencies
============

* An authenticated account.
* A Consumer Notebook API Key. If you don't have one, `please request an API Key`_.

.. _`please request an API Key`: http://consumernotebook.com/request-api-key/

Authentication
==============

All API calls require HTTP basic authentication and an API key::

    $ curl -u "username:PASSWORD" https://consumernotebook.com/api/v1/products.json?api_key=MYAPIKEY

Client Libraries
================

So far there's just a simple Python client library.  If you write a library for another language (or another Python client library for that matter), let us know and we'll link/credit you here.

Python:

* python-cn-client_ (alpha) -- by `Daniel Greenfeld`_

.. _python-cn-client: https://github.com/consumernotebook/python-cn-client
.. _`Daniel Greenfeld`: http://pydanny.com




