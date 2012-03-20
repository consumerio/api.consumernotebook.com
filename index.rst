Consumer Notebook API Documentation
===================================

Welcome!  Also see the Consumer Notebook Developer Center (`developers.consumernotebook.com`_) for our graphic identity kit, featured projects, and much more.

.. _`developers.consumernotebook.com`: http://developers.consumernotebook.com

REST API Features:

* Get Product, Grid, and List data as JSON responses.
* OAuth2 authentication so you/we can track usage.

First, read this:

.. toctree::
   :maxdepth: 2
   
   getting-started

   

Explore our REST API resources:

.. note:: The POST API will be launched around March 20th.

Products
==========

============================ ============================================================
Resource                     Description
============================ ============================================================
:ref:`api-v1-products`       Returns the most recent products added to Consumer Notebook.
:ref:`api-v1-product`        Returns the detail on a specific product.
:ref:`api-v1-schema`         Returns the structure of a Consumer Notebook product.
============================ ============================================================

Lists
==========

============================ ============================================================
Resource                     Description
============================ ============================================================
:ref:`api-v1-lists`          Returns the most recent lists modified.
:ref:`api-v1-list`           Returns the detail on a specific list.
============================ ============================================================

Grids
=====

============================ ============================================================
Resource                     Description
============================ ============================================================
:ref:`api-v1-grids`          Returns a list of grids in order they were created.
:ref:`api-v1-grid`           Returns the detail on a specific grid.
============================ ============================================================


Users
=====

============================ ============================================================
Resource                     Description
============================ ============================================================
:ref:`api-v1-users`          Returns a list of users.
:ref:`api-v1-user`           Returns the detail on a user.
:ref:`api-v1-user-schema`    Returns the structure of a Consumer Notebook user.
============================ ============================================================

----

Bookmarklet API
================

.. toctree::
 :maxdepth: 2

 bookmarklet-api


Table of Contents
=================

.. toctree::
    :maxdepth: 2

    api/v1/products
    api/v1/product
    api/v1/product_schema
    api/v1/lists
    api/v1/list
    api/v1/grids
    api/v1/grid
    api/v1/users
    api/v1/user
    api/v1/user_schema
    bookmarklet-api