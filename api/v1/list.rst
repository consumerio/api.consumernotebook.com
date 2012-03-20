.. _api-v1-list:

========================================
GET /api/v1/lists/{username}/{list_slug}
========================================

Returns the list described by the username and list slug.

Parameters
==========

access_token
    Oauth2 access token required for all Consumer Notebook REST API requests.
    
format (optional)
    * json (default)
    * jsonp
    
Example Request
================

Get::

    curl https://consumernotebook.com/api/v1/lists/pydanny/kinect-games/ -d access_token={access_token} -G
    
Results:    

.. sourcecode:: javascript

    {
        "created": "2012-03-08T22:17:42.952447",
        "description": "",
        "id": "532",
        "last_modified_by_user": "2012-03-08T17:07:56.810606",
        "modified": "2012-03-18T21:33:29.628668",
        "owner": {
            "avatar": "/media/avatars/pydanny/resized/80/avatars/pydanny/daniel.greenfeld.jpg",
            "coins": 122,
            "fullname": "Daniel Greenfelds",
            "score": 695,
            "username": "pydanny",
            "waitlisted": false
        },
        "products": [{
            "comment": "",
            "external_link": "http://www.amazon.com/gp/product/B0053BG370/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
            "id": "4f59a086204d33000e000000",
            "image_url": "http://ecx.images-amazon.com/images/I/61fezndpqNL.jpg",
            "link": "/motionsports-adrenaline-xbox/4f59a086204d33000e000000/",
            "price_range": "$50-100",
            "resource_uri": "/api/v1/products/4f59a086204d33000e000000/",
            "title": "MotionSports Adrenaline: XBox"
        },
        {
            "comment": "A super heroku fight game? Sign me up!",
            "external_link": "http://www.amazon.com/gp/product/B004U9T6FM/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
            "id": "4f59a0f55ddae9000d000000",
            "image_url": "http://ecx.images-amazon.com/images/I/61j1tcm6ZjL.jpg",
            "link": "/powerup-heroes-xbox/4f59a0f55ddae9000d000000/",
            "price_range": "$20-50",
            "resource_uri": "/api/v1/products/4f59a0f55ddae9000d000000/",
            "title": "PowerUP Heroes: XBox"
        },
        {
            "comment": "I like games",
            "external_link": "http://www.amazon.com/gp/product/B002I0H8FK/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
            "id": "4f5b9c9f24b4b3000e000003",
            "image_url": "http://ecx.images-amazon.com/images/I/5109BtpAZPL.jpg",
            "link": "/child-of-eden-xbox-360-video-games/4f5b9c9f24b4b3000e000003/",
            "price_range": "$20-50",
            "resource_uri": "/api/v1/products/4f5b9c9f24b4b3000e000003/",
            "title": "Child Of Eden: Xbox 360: Video Games"
        },
        {
            "comment": "deepak!",
            "external_link": "http://www.amazon.com/gp/product/B0056WJA3K/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
            "id": "4f5b9e1736a633000d000006",
            "image_url": "http://ecx.images-amazon.com/images/I/51llqktiEZL.jpg",
            "link": "/deepak-chopras-leela-xbox-360-video-games/4f5b9e1736a633000d000006/",
            "price_range": "$20-50",
            "resource_uri": "/api/v1/products/4f5b9e1736a633000d000006/",
            "title": "Deepak Chopra's Leela: Xbox 360: Video Games"
        },
        {
            "comment": "Dance!",
            "external_link": "http://www.amazon.com/gp/product/B00061NL7W/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
            "id": "4f5ba47936a633000e000006",
            "image_url": "http://ecx.images-amazon.com/images/I/51vm-es1RUL.jpg",
            "link": "/yourself-fitness-xbox/4f5ba47936a633000e000006/",
            "price_range": "$50-100",
            "resource_uri": "/api/v1/products/4f5ba47936a633000e000006/",
            "title": "Yourself Fitness: Xbox:"
        },
        {
            "comment": "guy is punching!",
            "external_link": "http://www.amazon.com/gp/product/B002I0H9WM/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
            "id": "4f5bab081cfd5d000c000008",
            "image_url": "http://ecx.images-amazon.com/images/I/51gcyDU9V%2BL.jpg",
            "link": "/your-shape-fitness-evolved-video-games/4f5bab081cfd5d000c000008/",
            "price_range": "$50-100",
            "resource_uri": "/api/v1/products/4f5bab081cfd5d000c000008/",
            "title": "Your Shape Fitness Evolved: Video Games"
        }],
        "resource_uri": "/api/v1/lists/pydanny/kinect-games/",
        "slug": "kinect-games",
        "title": "Kinect Games",
        "url": "http://consumernotebook.com/lists/pydanny/kinect-games/"
    }