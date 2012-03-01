===============
Bookmarklet API
===============

This is what receives the results of the Consumer Notebook bookmarklet. 

.. warning:: Use of this API to upload content that is inappropriate, obscene, illegal, or violates our terms and conditions can and will cause your account to be suspended without notice.

Dependencies
============

* An authenticated account.

Method
======

HTTP Get

Target
=======

.. parsed-literal::

    http://consumernotebook.com/add-product/
    
Parameters
==========

All of the following are required and must be URLEncoded.

========= ======== ======================================================
Name      Required Note
========= ======== ======================================================
title     Yes      The name of the product being added
url       Yes      The product URL, or where it is found on the Internet.
image_url Yes      The image used to display the product.
========= ======== ======================================================

Example
=======

.. parsed-literal::

    http://consumernotebook.com/add-product/?title=Kindle%20Fire%20-%20Full%20Color%207%22%20Multi-Touch%20Display%20with%20Wi-Fi%20-%20More%20than%20a%20Tablet&url=http%3A%2F%2Fwww.amazon.com%2Fdp%2FB0051VVOB2%2F&image_url=http%3A%2F%2Fg-ecx.images-amazon.com%2Fimages%2FG%2F01%2Fkindle%2Fotter%2Fdp%2FKO-details-right._V166939146_.jpg