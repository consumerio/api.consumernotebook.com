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

Products
==========

============================ ============================================================
Resource                     Description
============================ ============================================================
:ref:`api-v1-my-products`    Returns a list of products you've bookmarked
:ref:`api-v1-products`       Returns the most recent products added to Consumer Notebook.
:ref:`api-v1-product`        Returns the detail on a specific product.
:ref:`api-v1-schema`         Returns the structure of a Consumer Notebook product.
:ref:`api-v1-post-product`   Adds or bookmarks a product
============================ ============================================================

Lists
==========

=============================== ============================================================
Resource                        Description
=============================== ============================================================
:ref:`api-v1-my-lists`          Returns your lists
:ref:`api-v1-lists`             Returns the most recent lists modified.
:ref:`api-v1-list`              Returns the detail on a specific list.
:ref:`api-v1-post-manage-lists` Adds a list. The list is the property of the creating user.
=============================== ============================================================

Grids
=====

============================ ============================================================
Resource                     Description
============================ ============================================================
:ref:`api-v1-my-grids`       Returns your grids
:ref:`api-v1-grids`          Returns a list of grids in order they were created.
:ref:`api-v1-grid`           Returns the detail on a specific grid.
============================ ============================================================


Users
=====

============================= ============================================================
Resource                      Description
============================= ============================================================
:ref:`api-v1-my-profile`      Returns your profile
:ref:`api-v1-users`           Returns a list of users.
:ref:`api-v1-user`            Returns the detail on a user.
:ref:`api-v1-user-schema`     Returns the structure of a Consumer Notebook user.
:ref:`api-v1-put-my-profile`  Update your profile
============================= ============================================================


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

    api/v1/my-products
    api/v1/products
    api/v1/product
    api/v1/product_schema
    api/v1/post-product
    api/v1/my-lists
    api/v1/lists
    api/v1/list
    api/v1/post-manage-lists
    api/v1/my-grids
    api/v1/grids
    api/v1/grid
    api/v1/my-profile
    api/v1/users
    api/v1/user
    api/v1/user_schema
    api/v1/put-my-profile
    bookmarklet-api