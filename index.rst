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
GET api/v1/products/         Returns the most recent products added to Consumer Notebook. 
GET /api/v1/products/<pk>/   Returns the detail on a specific product.
GET /api/v1/products/schema/ Returns the structure of a Consumer Notebook product.
============================ ============================================================

Lists
==========

============================ ============================================================
Resource                     Description
============================ ============================================================
GET /api/v1/lists/           Returns the most recent lists modified.
GET /api/v1/lists/<pk>/      Returns the detail on a specific lists.
GET /api/v1/lists/schema/    Returns the structure of a Consumer Notebook list.
============================ ============================================================

.. toctree::
   :maxdepth: 2

   api/products-api
   api/lists-api
   api/grids-api
   api/users-api
   api/bookmarklet-api

