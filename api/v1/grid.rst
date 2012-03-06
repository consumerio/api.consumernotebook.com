.. _api-v1-grid:

======================
GET /api/v1/grids/{id}
======================

Returns the specified ``grid`` resource.

Parameters
==========

apikey
    Required for all Consumer Notebook REST API requests. You can also place this in the HTTP_AUTHORIZATION header.

format (optional)
    * json (default)
    * jsonp


Example Request
================

Get::

    curl https://consumernotebook.com/api/v1/grids/4f319564bf8bbd000a000000/ -d apikey={apikey} -G
    
Results:    

.. sourcecode:: javascript

    {
        "features": [
        {
                "description": "Five great books on which to build up your Python knowledge.",
                "slug": "rating",
                "title": "rating"
            },
            {
                "description": "",
                "slug": "author",
                "title": "author"
            },
            {
                "description": "",
                "slug": "expert-friendliness",
                "title": "Expert Friendliness"
            },
            {
                "description": "",
                "slug": "beginner-friendliness",
                "title": "Beginner Friendliness"
            },
            {
                "description": "",
                "slug": "note",
                "title": "note"
            }
        ],
        "grid_items": [
            {
                "created": "2012-02-07T13:19:45.495000",
                "elements": {
                    "author": "Mark Lutz",
                    "beginner-friendliness": "[emote-4]",
                    "expert-friendliness": "[emote-4]",
                    "note": "I have this weird thing about good pocket references - I find them as useful for learning things about tools as I do the monstrous tomes. This qualifies as one of those super useful references that justifies a purchase. You can't go wrong with this, especially considering the price. Great for picking up core Python built-ins as well as all the the awesome methods on the native types.",
                    "rating": "[star-5]"
                },
                "id": "4f3c019eebae2600040001bc"
            },
            {
                "created": "2012-02-07T13:20:39.672000",
                "elements": {
                    "author": "David Beazley",
                    "beginner-friendliness": "[emote-4]",
                    "expert-friendliness": "[emote-5]",
                    "note": "In any case, this is a great book for programming in Python. It is a library by library reference for programming in Python. In quiet moments I used to slow peruse the pages to make sure I knew all the great bits that Python gives me out of of the box.",
                    "rating": "[star-5]"
                },
                "id": "4f3c0176ebae2600040000d8"
            },
            {
                "created": "2012-02-07T13:20:53.671000",
                "elements": {
                    "author": "Doug Hellmann",
                    "beginner-friendliness": "[emote-4]",
                    "expert-friendliness": "[emote-5]",
                    "note": "Released in early 2011, this is an enormous book but nearly worth the weight. Think of it as combining the cookbook and essential reference and you've got an idea as to what this book gives you. This book is unbelievable in it's depth and quality. The downside of this book is it's gigantic size. I would have liked to have seen this broken up into two volumes.",
                    "rating": "[star-4.5]"
                },
                "id": "4f3c016bebae2600040000bc"
            },
            {
                "created": "2012-02-07T13:20:23.067000",
                "elements": {
                    "author": "Alex Martelli, Anna Ravenscroft, David Ascher",
                    "beginner-friendliness": "[emote-4]",
                    "expert-friendliness": "[emote-4]",
                    "note": "This will get bumped to 5 stars when it's modernized! Being a series of recipes for solving various problems in Python, this is an amazing, wonderful book. In 2006 for the holidays I landed two copies as presents, and the book is so good I kept them both. One for the office and one for home! This is a great reference and full of wonderful gems and tricks for Python developers of all types.",
                    "rating": "[star-4]"
                },
                "id": "4f3c01a7ebae260004000235"
            },
            {
                "created": "2012-02-07T13:20:04.829000",
                "elements": {
                    "author": "Mark Lutz",
                    "beginner-friendliness": "[emote-5]",
                    "expert-friendliness": "[emote-4]",
                    "note": "In 2005 I learned Python from the 2003 edition of this book. Most of it was great and quite useful, except for the three chapters on Jython. Other people swear by Dive into Python but I found this a much clearer way to get into the language. These days I recommend Zed Shaw's Learn Python the Hard Way, but this is still a good resource for beginning Python developers.",
                    "rating": "[star-4]"
                },
                "id": "4f3c0177ebae2600040000f1"
            }
        ],
        "id": "4f319564bf8bbd000a000000",
        "last_modified_by_user": "2012-02-23T15:28:14.892000",
        "resource_uri": "/api/v1/grids/4f319564bf8bbd000a000000/",
        "title": "Must-Have Python Programming Books ",
        "username": "pydanny"
    }