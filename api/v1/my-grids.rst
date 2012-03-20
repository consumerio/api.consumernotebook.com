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
            "next": "/api/v1/my-grids/?access_token={access_token}&limit=20&offset=20",
            "offset": 0,
            "previous": null,
            "total_count": 116
        },
        "objects": [{
            "id": "4f665f139007d7000d000002",
            "last_modified_by_user": "2012-03-18T16:23:49.058000",
            "resource_uri": "/api/v1/my-grids/michaelwarkentin/heroku-mail-addons/",
            "slug": "heroku-mail-addons",
            "title": "Heroku Mail Addons",
            "url": "http://consumernotebook.com/grids/michaelwarkentin/heroku-mail-addons/",
            "username": "michaelwarkentin"
        },
        {
            "id": "4f64f5f2555803000e00000b",
            "last_modified_by_user": "2012-03-17T14:08:24.081000",
            "resource_uri": "/api/v1/my-grids/tlesher/gas-grills-under-500/",
            "slug": "gas-grills-under-500",
            "title": "Gas Grills under $500",
            "url": "http://consumernotebook.com/grids/tlesher/gas-grills-under-500/",
            "username": "tlesher"
        },
        {
            "id": "4f64d708555803000e000004",
            "last_modified_by_user": "2012-03-17T11:27:57.332000",
            "resource_uri": "/api/v1/my-grids/frogmonkey/monitor-24/",
            "slug": "monitor-24",
            "title": "Monitor -24\"",
            "url": "http://consumernotebook.com/grids/frogmonkey/monitor-24/",
            "username": "frogmonkey"
        },
        {
            "id": "4f64d5cf555803000e000002",
            "last_modified_by_user": "2012-03-17T11:23:43.444000",
            "resource_uri": "/api/v1/my-grids/jaredahardy/electric-or-hybrid-cars/",
            "slug": "electric-or-hybrid-cars",
            "title": "Electric or hybrid cars",
            "url": "http://consumernotebook.com/grids/jaredahardy/electric-or-hybrid-cars/",
            "username": "jaredahardy"
        },
        {
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
            "id": "4f5b728224b4b3000e000002",
            "last_modified_by_user": "2012-03-10T07:27:01.622000",
            "resource_uri": "/api/v1/my-grids/moskrc/test/",
            "slug": "test",
            "title": "Test",
            "url": "http://consumernotebook.com/grids/moskrc/test/",
            "username": "moskrc"
        },
        {
            "id": "4f5ae3f636a633000d000004",
            "last_modified_by_user": "2012-03-11T01:41:59.950000",
            "resource_uri": "/api/v1/my-grids/regebro/elliptical-trainers/",
            "slug": "elliptical-trainers",
            "title": "Elliptical trainers",
            "url": "http://consumernotebook.com/grids/regebro/elliptical-trainers/",
            "username": "regebro"
        },
        {
            "id": "4f5ae0dd24b4b3000d000000",
            "last_modified_by_user": "2012-03-09T21:17:40.316000",
            "resource_uri": "/api/v1/my-grids/dgreenfeld/diatomaceous-earth/",
            "slug": "diatomaceous-earth",
            "title": "diatomaceous earth",
            "url": "http://consumernotebook.com/grids/dgreenfeld/diatomaceous-earth/",
            "username": "dgreenfeld"
        },
        {
            "id": "4f555f867428cd000c000000",
            "last_modified_by_user": "2012-03-05T17:00:51.469000",
            "resource_uri": "/api/v1/my-grids/audreyr/vanilla-beans/",
            "slug": "vanilla-beans",
            "title": "Vanilla Beans",
            "url": "http://consumernotebook.com/grids/audreyr/vanilla-beans/",
            "username": "audreyr"
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
            "id": "4f553b0d2f68b5000d000004",
            "last_modified_by_user": "2012-03-05T15:08:14.682000",
            "resource_uri": "/api/v1/my-grids/esacteksab/color-e-reader/",
            "slug": "color-e-reader",
            "title": "Color E-Reader",
            "url": "http://consumernotebook.com/grids/esacteksab/color-e-reader/",
            "username": "esacteksab"
        },
        {
            "id": "4f5537a54fa437000c000001",
            "last_modified_by_user": "2012-03-05T14:05:30.723000",
            "resource_uri": "/api/v1/my-grids/esacteksab/mens-body-wash/",
            "slug": "mens-body-wash",
            "title": "Men's Body Wash",
            "url": "http://consumernotebook.com/grids/esacteksab/mens-body-wash/",
            "username": "esacteksab"
        },
        {
            "id": "4f5414ff29566a000e000001",
            "last_modified_by_user": "2012-03-04T17:21:03.632000",
            "resource_uri": "/api/v1/my-grids/paulhildebrandt/property-management/",
            "slug": "property-management",
            "title": "Property Management",
            "url": "http://consumernotebook.com/grids/paulhildebrandt/property-management/",
            "username": "paulhildebrandt"
        },
        {
            "id": "4f53db374a103e000e000000",
            "last_modified_by_user": "2012-03-04T13:19:55.282000",
            "resource_uri": "/api/v1/my-grids/audreyr/outdoor-bike-storage-sheds/",
            "slug": "outdoor-bike-storage-sheds",
            "title": "Outdoor Bike Storage Sheds",
            "url": "http://consumernotebook.com/grids/audreyr/outdoor-bike-storage-sheds/",
            "username": "audreyr"
        },
        {
            "id": "4f5391763686ec000e000000",
            "last_modified_by_user": "2012-03-04T07:59:50.186000",
            "resource_uri": "/api/v1/my-grids/boardman/monitor-arms/",
            "slug": "monitor-arms",
            "title": "Monitor Arms",
            "url": "http://consumernotebook.com/grids/boardman/monitor-arms/",
            "username": "boardman"
        },
        {
            "id": "4f4ed8a34a8422000d000003",
            "last_modified_by_user": "2012-03-12T17:25:40.322000",
            "resource_uri": "/api/v1/my-grids/shawnr/2011-handheld-game-consoles/",
            "slug": "2011-handheld-game-consoles",
            "title": "2011 Handheld Game Consoles",
            "url": "http://consumernotebook.com/grids/shawnr/2011-handheld-game-consoles/",
            "username": "shawnr"
        },
        {
            "id": "4f4e99614a8422000c000006",
            "last_modified_by_user": "2012-03-04T19:32:32.250000",
            "resource_uri": "/api/v1/my-grids/mark0978/what-is-this/",
            "slug": "what-is-this",
            "title": "What is this?",
            "url": "http://consumernotebook.com/grids/mark0978/what-is-this/",
            "username": "mark0978"
        },
        {
            "id": "4f4e8aefcac041000d000002",
            "last_modified_by_user": "2012-03-09T17:03:15.039000",
            "resource_uri": "/api/v1/my-grids/audreyr/apple-tv-vs-google-tv-vs-roku-vs-boxee/",
            "slug": "apple-tv-vs-google-tv-vs-roku-vs-boxee",
            "title": "Apple TV vs. Google TV vs. Roku vs. Boxee",
            "url": "http://consumernotebook.com/grids/audreyr/apple-tv-vs-google-tv-vs-roku-vs-boxee/",
            "username": "audreyr"
        },
        {
            "id": "4f4e853d4a8422000d000001",
            "last_modified_by_user": "2012-02-29T12:11:52.906000",
            "resource_uri": "/api/v1/my-grids/magicsword/arduino/",
            "slug": "arduino",
            "title": "Arduino",
            "url": "http://consumernotebook.com/grids/magicsword/arduino/",
            "username": "magicsword"
        }]
    }