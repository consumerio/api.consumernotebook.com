Consumer Notebook API Documentation
===================================

Welcome!  Also see the Consumer Notebook Developer Center (`developers.consumernotebook.com`_) for our graphic identity kit, featured projects, and much more.

.. _`developers.consumernotebook.com`: http://developers.consumernotebook.com

REST API Features:

* Get Product, Grid, and List data via our REST API.
* API Keys so you/we can track usage.

.. warning:: This is not yet activated on the site. Any and all requests against it will fail until we officially release this at PyCon 2012!


First, read this:

.. toctree::
   :maxdepth: 2
   
   getting-started

Then explore our REST API resources:

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
:ref:`api-v1-list`           Returns the detail on a specific lists.
:ref:`api-v1-list-schema`    Returns the structure of a Consumer Notebook list.
============================ ============================================================

Grids
=====

============================ ============================================================
Resource                     Description
============================ ============================================================
:ref:`api-v1-grids`          Returns a list of grids in order they were created.
GET /api/v1/grids/{id}/      Returns the detail on a specific grid.
:ref:`api-v1-grid-schema`    Returns the structure of a Consumer Notebook grid.
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

Resources Table of Contents
============================

.. toctree::
   :maxdepth: 2
   
   api/v1/products
   api/v1/product
   api/v1/product_schema
   api/v1/lists
   api/v1/list
   api/v1/list_schema
   api/v1/grids
   api/v1/grid_schema   
   api/v1/users
   api/v1/user
   api/v1/user_schema       
   
Old API Docs
============

.. toctree::
   :maxdepth: 2

   old_api/products-api
   old_api/lists-api
   old_api/grids-api
   old_api/users-api
   old_api/bookmarklet-api

