.. _api-v1-lists:

=====================
GET /api/v1/lists/
=====================

Returns the most recent lists added to Consumer Notebook.  This method is can only return up to 20 lists at a time.

Parameters
==========

apikey
    Required for all Consumer Notebook REST API requests. You can also place this in the HTTP_AUTHORIZATION header.

format (optional)
    * json (default)
    * jsonp
    
offset (optional)
    Specifies the page of results to retrieve. Defaults to 0.

Example Request
================

Get::

    curl https://consumernotebook.com/api/v1/lists/ -d apikey={apikey} -G
    
Results:    

.. sourcecode:: javascript

    {
        "meta": {
            "limit": 20,
            "next": "/api/v1/lists/?apikey={apikey}&limit=20&offset=20",
            "offset": 0,
            "previous": null,
            "total_count": 232
        },
        "objects": [
            {
                "created": "2012-03-05T12:57:49.696813",
                "description": "List of resources for Scrum",
                "id": "524",
                "last_modified_by_user": "2012-03-05T09:29:54.425210",
                "modified": "2012-03-05T12:57:49.707313",
                "owner": {
                    "avatar": "https://consumernotebook.s3.amazonaws.com/avatars/paulhildebrandt/resized/80/avatars/paulhildebrandt/Profile.jpg",
                    "coins": 0,
                    "fullname": "Paul Hildebrandt",
                    "score": 4,
                    "username": "paulhildebrandt",
                    "waitlisted": false
                },
                "products": [{
                    "created": "2012-03-05T12:58:15.492404",
                    "modified": "2012-03-05T12:58:15.518605",
                    "order": 0,
                    "product": {
                        "_id": "4f5528644fa437000d000000",
                        "creator": "paulhildebrandt",
                        "image_url": null,
                        "price_range": 100,
                        "title": "A Book of Five Rings: The Strategy of Musashi (Audible Audio Edition)",
                        "url": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.amazon.com/gp/product/B004IDNS6S"
                    },
                    "reason": "Good Product Owner book",
                    "resource_uri": ""
                }],
                "resource_uri": "/api/v1/lists/524/",
                "slug": "scrum",
                "title": "Scrum"
            },
            {
                "created": "2012-03-04T21:47:02.773453",
                "description": "It can be hard to buy gifts for an active, retired mom. These are nice, affordable gifts any mother would love.",
                "id": "523",
                "last_modified_by_user": "2012-03-04T22:15:18.861270",
                "modified": "2012-03-04T22:15:18.945776",
                "owner": {
                    "avatar": "/media/avatars/pydanny/resized/80/avatars/pydanny/daniel.greenfeld.jpg",
                    "coins": 122,
                    "fullname": "Daniel Greenfeld",
                    "score": 685,
                    "username": "pydanny",
                    "waitlisted": false
                },
                "products": [{
                    "created": "2012-03-04T21:51:40.127375",
                    "modified": "2012-03-04T21:51:40.156011",
                    "order": 1,
                    "product": {
                        "_id": "4f54546cb15ef7000e000002",
                        "creator": "pydanny",
                        "image_url": "http://ecx.images-amazon.com/images/I/41i3G25PRZL.jpg",
                        "price_range": 50,
                        "title": "Aurorae Classic Yoga Mat - Always smells good.",
                        "url": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.amazon.com/gp/product/B004TN51EE"
                    },
                    "reason": "Yoga has been taken up by a lot of active, retired moms. This mat stays odor free pretty much forever, and is thick enough to keep joints off cold, hard floors.",
                    "resource_uri": ""
                },
                {
                    "created": "2012-03-04T22:14:55.600677",
                    "modified": "2012-03-04T22:14:55.630535",
                    "order": 3,
                    "product": {
                        "_id": "4f5459dfb15ef7000c000006",
                        "creator": "pydanny",
                        "image_url": "http://www.flowersacrossamerica.com/flowers/products/C26-2943.jpg",
                        "price_range": 100,
                        "title": "French Garden - Best Selling Flowers",
                        "url": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.flowersacrossamerica.com/product.cfm%3Fdcode%3DC26-2943"
                    },
                    "reason": "Because of their longevity, moms often prefer plants over flowers. ",
                    "resource_uri": ""
                },
                {
                    "created": "2012-03-04T21:49:19.182313",
                    "modified": "2012-03-04T22:15:08.926987",
                    "order": 3,
                    "product": {
                        "_id": "4f5453dfb15ef7000e000000",
                        "creator": "pydanny",
                        "image_url": "http://ecx.images-amazon.com/images/I/41%2Bz99pmfVL.jpg",
                        "price_range": 50,
                        "title": "Akro-Mils Stack-A-Pot",
                        "url": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.amazon.com/gp/product/B002IYHIKG"
                    },
                    "reason": "This is great for any garden, large or small. Mom can pack in a lot of herbs or flowers into a small location in a very attractive package.",
                    "resource_uri": ""
                },
            ],
            ...
        ],
        ...
    }