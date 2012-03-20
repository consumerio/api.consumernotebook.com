.. _api-v1-my-grids:

=======================
GET /api/v1/my-grids/
=======================

Returns your grids.

Parameters
==========

access_token
    OAuth2 access token required for all Consumer Notebook REST API requests.

format (optional)
    * json (default)
    * jsonp
    

Example Request
================

Get::

    curl https://consumernotebook.com/api/v1/my-grids/ -d access_token={access_token} -G
    
Results:    

.. sourcecode:: javascript

    {
        "meta": {
            "limit": 20,
            "next": null,
            "offset": 0,
            "previous": null,
            "total_count": 17
        },
        "objects": [{
            "id": "4f615025e0eac7000c00000c",
            "last_modified_by_user": "2012-03-18T17:20:58.240000",
            "resource_uri": "/api/v1/my-grids/pydanny/super-cheap-cell-phones/",
            "slug": "super-cheap-cell-phones",
            "title": "Super Cheap Cell Phones",
            "url": "http://consumernotebook.com/grids/pydanny/super-cheap-cell-phones/",
            "username": "pydanny"
        },
        {
            "id": "4f5bb18b1cfd5d000e000003",
            "last_modified_by_user": "2012-03-18T17:10:26.053000",
            "resource_uri": "/api/v1/my-grids/pydanny/camping-lanterns/",
            "slug": "camping-lanterns",
            "title": "camping lanterns",
            "url": "http://consumernotebook.com/grids/pydanny/camping-lanterns/",
            "username": "pydanny"
        },
        {
            "id": "4f555f83247c21000d000001",
            "last_modified_by_user": "2012-03-05T16:51:15.957000",
            "resource_uri": "/api/v1/my-grids/pydanny/doctor-who-holiday-specials/",
            "slug": "doctor-who-holiday-specials",
            "title": "Doctor Who Holiday Specials",
            "url": "http://consumernotebook.com/grids/pydanny/doctor-who-holiday-specials/",
            "username": "pydanny"
        },
        {
            "id": "4f4c6df09acecc000e000002",
            "last_modified_by_user": "2012-03-14T19:09:40.791000",
            "resource_uri": "/api/v1/my-grids/pydanny/best-wireless-routers/",
            "slug": "best-wireless-routers",
            "title": "Best Wireless Routers",
            "url": "http://consumernotebook.com/grids/pydanny/best-wireless-routers/",
            "username": "pydanny"
        },
        {
            "id": "4f4977cfbebb78000e000003",
            "last_modified_by_user": "2012-02-25T16:12:33.701000",
            "resource_uri": "/api/v1/my-grids/pydanny/my-pycon-startup-row-shoe-options/",
            "slug": "my-pycon-startup-row-shoe-options",
            "title": "My PyCon Startup Row shoe options",
            "url": "http://consumernotebook.com/grids/pydanny/my-pycon-startup-row-shoe-options/",
            "username": "pydanny"
        },
        {
            "id": "4f4951976721be000e000003",
            "last_modified_by_user": "2012-02-26T01:41:30.861000",
            "resource_uri": "/api/v1/my-grids/pydanny/vita-games/",
            "slug": "vita-games",
            "title": "Vita Games",
            "url": "http://consumernotebook.com/grids/pydanny/vita-games/",
            "username": "pydanny"
        },
        {
            "id": "4f455cb8ee02ef000b000000",
            "last_modified_by_user": "2012-02-22T13:26:08.954000",
            "resource_uri": "/api/v1/my-grids/pydanny/hybrid-cars/",
            "slug": "hybrid-cars",
            "title": "Hybrid Cars",
            "url": "http://consumernotebook.com/grids/pydanny/hybrid-cars/",
            "username": "pydanny"
        },
        {
            "id": "4f4164cbf5484c000c000001",
            "last_modified_by_user": "2012-03-14T15:46:33.143000",
            "resource_uri": "/api/v1/my-grids/pydanny/trampolines/",
            "slug": "trampolines",
            "title": "Trampolines",
            "url": "http://consumernotebook.com/grids/pydanny/trampolines/",
            "username": "pydanny"
        },
        {
            "id": "4f3da271b46d8f000c000000",
            "last_modified_by_user": "2012-03-01T21:08:56.199000",
            "resource_uri": "/api/v1/my-grids/pydanny/deluxe-spring-water/",
            "slug": "deluxe-spring-water",
            "title": "Deluxe Spring Water",
            "url": "http://consumernotebook.com/grids/pydanny/deluxe-spring-water/",
            "username": "pydanny"
        },
        {
            "id": "4f3c4f425b99b2000b000001",
            "last_modified_by_user": "2012-03-18T17:20:58.238000",
            "resource_uri": "/api/v1/my-grids/pydanny/python-books-for-beginners/",
            "slug": "python-books-for-beginners",
            "title": "Python books for beginners",
            "url": "http://consumernotebook.com/grids/pydanny/python-books-for-beginners/",
            "username": "pydanny"
        },
        {
            "id": "4f3c1edebe4aee000a000000",
            "last_modified_by_user": "2012-02-15T15:12:26.233000",
            "resource_uri": "/api/v1/my-grids/pydanny/economy-cars/",
            "slug": "economy-cars",
            "title": "Economy Cars",
            "url": "http://consumernotebook.com/grids/pydanny/economy-cars/",
            "username": "pydanny"
        },
        {
            "id": "4f377ffa5ac429000b000000",
            "last_modified_by_user": "2012-02-15T12:38:20.231000",
            "resource_uri": "/api/v1/my-grids/pydanny/heaters/",
            "slug": "heaters",
            "title": "Heaters",
            "url": "http://consumernotebook.com/grids/pydanny/heaters/",
            "username": "pydanny"
        },
        {
            "id": "4f319564bf8bbd000a000000",
            "last_modified_by_user": "2012-03-14T19:02:27.612000",
            "resource_uri": "/api/v1/my-grids/pydanny/must-have-python-programming-books/",
            "slug": "must-have-python-programming-books",
            "title": "Must-Have Python Programming Books ",
            "url": "http://consumernotebook.com/grids/pydanny/must-have-python-programming-books/",
            "username": "pydanny"
        },
        {
            "id": "4f3088db39006c000a000000",
            "last_modified_by_user": "2012-02-09T19:47:37.085000",
            "resource_uri": "/api/v1/my-grids/pydanny/wacky-pajamas/",
            "slug": "wacky-pajamas",
            "title": "Wacky Pajamas",
            "url": "http://consumernotebook.com/grids/pydanny/wacky-pajamas/",
            "username": "pydanny"
        },
        {
            "id": "4f303fafd52246000b000000",
            "last_modified_by_user": "2012-02-07T18:53:26.325000",
            "resource_uri": "/api/v1/my-grids/pydanny/django-books-2/",
            "slug": "django-books-2",
            "title": "Django Books 2",
            "url": "http://consumernotebook.com/grids/pydanny/django-books-2/",
            "username": "pydanny"
        },
        {
            "id": "4f300cfb5b5915000b000000",
            "last_modified_by_user": "2012-02-06T17:11:59.653000",
            "resource_uri": "/api/v1/my-grids/pydanny/technical-martial-arts-movies-1/",
            "slug": "technical-martial-arts-movies-1",
            "title": "Technical Martial Arts Movies 1",
            "url": "http://consumernotebook.com/grids/pydanny/technical-martial-arts-movies-1/",
            "username": "pydanny"
        },
        {
            "id": "4f2ff7882570ad000b000000",
            "last_modified_by_user": "2012-03-01T21:07:31.652000",
            "resource_uri": "/api/v1/my-grids/pydanny/django-books-1/",
            "slug": "django-books-1",
            "title": "Django Books 1",
            "url": "http://consumernotebook.com/grids/pydanny/django-books-1/",
            "username": "pydanny"
        }]
    }