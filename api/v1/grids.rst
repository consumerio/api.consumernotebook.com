.. _api-v1-grids:

=====================
GET /api/v1/grids/
=====================

Returns the most recent grids added to Consumer Notebook.  This method is can only return up to 20 grids at a time.

Parameters
==========

apikey
    Required for all Consumer Notebook REST API requests. You can also place this in the HTTP_AUTHORIZATION header.

format (optional)
    * json (default)
    * jsonp
    
offset (optional)
    Specifies the page of results to retrieve. Defaults to 0.
    
username (optional)
    This filters by username.
    

Example Request
================

Get::

    curl https://consumernotebook.com/api/v1/grids/ -d apikey={apikey} -d username=audreyr -G
    
Results:    

.. sourcecode:: javascript

    {
        "meta": {
            "limit": 20,
            "next": "/api/v1/grids/?depth=1&apikey={apikey}&limit=20&offset=20",
            "offset": 0,
            "previous": null,
            "total_count": 107
        },
        "objects": [
            {
                "id": "4f555f867428cd000c000000",
                "last_modified_by_user": "2012-03-05T17:00:51.469000",
                "resource_uri": "/api/v1/grids/4f555f867428cd000c000000/",
                "slug": "vanilla-beans",
                "title": "Vanilla Beans",
                "url": "http://consumernotebook.com/grids/audreyr/vanilla-beans/",
                "username": "audreyr"
            },
            {
                "id": "4f555f83247c21000d000001",
                "last_modified_by_user": "2012-03-05T16:51:15.957000",
                "resource_uri": "/api/v1/grids/4f555f83247c21000d000001/",
                "slug": "doctor-who-holiday-specials",
                "title": "Doctor Who Holiday Specials",
                "url": "http://consumernotebook.com/grids/pydanny/doctor-who-holiday-specials/",
                "username": "pydanny"
            },
            {
                "id": "4f553b0d2f68b5000d000004",
                "last_modified_by_user": "2012-03-05T15:08:14.682000",
                "resource_uri": "/api/v1/grids/4f553b0d2f68b5000d000004/",
                "slug": "color-e-reader",
                "title": "Color E-Reader",
                "url": "http://consumernotebook.com/grids/esacteksab/color-e-reader/",
                "username": "esacteksab"
            },
            {
                "id": "4f5537a54fa437000c000001",
                "last_modified_by_user": "2012-03-05T14:05:30.723000",
                "resource_uri": "/api/v1/grids/4f5537a54fa437000c000001/",
                "slug": "mens-body-wash",
                "title": "Men's Body Wash",
                "url": "http://consumernotebook.com/grids/esacteksab/mens-body-wash/",
                "username": "esacteksab"
            },
            {
                "id": "4f5414ff29566a000e000001",
                "last_modified_by_user": "2012-03-04T17:21:03.632000",
                "resource_uri": "/api/v1/grids/4f5414ff29566a000e000001/",
                "slug": "property-management",
                "title": "Property Management",
                "url": "http://consumernotebook.com/grids/paulhildebrandt/property-management/",
                "username": "paulhildebrandt"
            },
            {
                "id": "4f53db374a103e000e000000",
                "last_modified_by_user": "2012-03-04T13:19:55.282000",
                "resource_uri": "/api/v1/grids/4f53db374a103e000e000000/",
                "slug": "outdoor-bike-storage-sheds",
                "title": "Outdoor Bike Storage Sheds",
                "url": "http://consumernotebook.com/grids/audreyr/outdoor-bike-storage-sheds/",
                "username": "audreyr"
            },
            {
                "id": "4f5391763686ec000e000000",
                "last_modified_by_user": "2012-03-04T07:59:50.186000",
                "resource_uri": "/api/v1/grids/4f5391763686ec000e000000/",
                "slug": "monitor-arms",
                "title": "Monitor Arms",
                "url": "http://consumernotebook.com/grids/boardman/monitor-arms/",
                "username": "boardman"
            },
            {
                "id": "4f4ed8a34a8422000d000003",
                "last_modified_by_user": "2012-02-29T18:46:54.213000",
                "resource_uri": "/api/v1/grids/4f4ed8a34a8422000d000003/",
                "slug": "2011-handheld-game-consoles",
                "title": "2011 Handheld Game Consoles",
                "url": "http://consumernotebook.com/grids/shawnr/2011-handheld-game-consoles/",
                "username": "shawnr"
            },
            {
                "id": "4f4e99614a8422000c000006",
                "last_modified_by_user": "2012-03-04T19:32:32.250000",
                "resource_uri": "/api/v1/grids/4f4e99614a8422000c000006/",
                "slug": "what-is-this",
                "title": "What is this?",
                "url": "http://consumernotebook.com/grids/mark0978/what-is-this/",
                "username": "mark0978"
            },
            {
                "id": "4f4e8aefcac041000d000002",
                "last_modified_by_user": "2012-02-29T15:11:06.182000",
                "resource_uri": "/api/v1/grids/4f4e8aefcac041000d000002/",
                "slug": "apple-tv-vs-google-tv-vs-roku-vs-boxee",
                "title": "Apple TV vs. Google TV vs. Roku vs. Boxee",
                "url": "http://consumernotebook.com/grids/audreyr/apple-tv-vs-google-tv-vs-roku-vs-boxee/",
                "username": "audreyr"
            },
            {
                "id": "4f4e853d4a8422000d000001",
                "last_modified_by_user": "2012-02-29T12:11:52.906000",
                "resource_uri": "/api/v1/grids/4f4e853d4a8422000d000001/",
                "slug": "arduino",
                "title": "Arduino",
                "url": "http://consumernotebook.com/grids/magicsword/arduino/",
                "username": "magicsword"
            },
            {
                "id": "4f4dd6b24a8422000c000002",
                "last_modified_by_user": "2012-02-28T23:41:38.981000",
                "resource_uri": "/api/v1/grids/4f4dd6b24a8422000c000002/",
                "slug": "test",
                "title": "test",
                "url": "http://consumernotebook.com/grids/fougazi/test/",
                "username": "fougazi"
            },
            {
                "id": "4f4d0546a84dd9000c000005",
                "last_modified_by_user": "2012-02-28T09:02:35.749000",
                "resource_uri": "/api/v1/grids/4f4d0546a84dd9000c000005/",
                "slug": "fridges-that-work-as-cheese-caves",
                "title": "Fridges That Work As Cheese Caves",
                "url": "http://consumernotebook.com/grids/audreyr/fridges-that-work-as-cheese-caves/",
                "username": "audreyr"
            },
            {
                "id": "4f4c6df09acecc000e000002",
                "last_modified_by_user": "2012-02-27T22:18:27.268000",
                "resource_uri": "/api/v1/grids/4f4c6df09acecc000e000002/",
                "slug": "best-wireless-routers",
                "title": "Best Wireless Routers",
                "url": "http://consumernotebook.com/grids/pydanny/best-wireless-routers/",
                "username": "pydanny"
            },
            {
                "id": "4f4c6cc2a1b3be000d000001",
                "last_modified_by_user": "2012-02-27T22:00:16.285000",
                "resource_uri": "/api/v1/grids/4f4c6cc2a1b3be000d000001/",
                "slug": "240-gb-ssd",
                "title": "240 GB SSD",
                "url": "http://consumernotebook.com/grids/frogmonkey/240-gb-ssd/",
                "username": "frogmonkey"
            },
            {
                "id": "4f4c6990611f84000d000005",
                "last_modified_by_user": "2012-02-27T21:43:44.056000",
                "resource_uri": "/api/v1/grids/4f4c6990611f84000d000005/",
                "slug": "pc-laptops-i7",
                "title": "PC Laptops i7",
                "url": "http://consumernotebook.com/grids/frogmonkey/pc-laptops-i7/",
                "username": "frogmonkey"
            },
            {
                "id": "4f4c58a99cab18000c000000",
                "last_modified_by_user": "2012-02-27T21:43:16.470000",
                "resource_uri": "/api/v1/grids/4f4c58a99cab18000c000000/",
                "slug": "cheesemaking-kits",
                "title": "Cheesemaking Kits",
                "url": "http://consumernotebook.com/grids/audreyr/cheesemaking-kits/",
                "username": "audreyr"
            },
            {
                "id": "4f49fd0258d56d000e000001",
                "last_modified_by_user": "2012-02-27T09:44:46.297000",
                "resource_uri": "/api/v1/grids/4f49fd0258d56d000e000001/",
                "slug": "stylish-unisex-camera-bags",
                "title": "Stylish Unisex Camera Bags",
                "url": "http://consumernotebook.com/grids/audreyr/stylish-unisex-camera-bags/",
                "username": "audreyr"
            },
            {
                "id": "4f49f910251fca000c000001",
                "last_modified_by_user": "2012-02-26T01:19:12.799000",
                "resource_uri": "/api/v1/grids/4f49f910251fca000c000001/",
                "slug": "womens-wallets-styled-like-mens-wallets",
                "title": "Women's Wallets Styled Like Men's Wallets",
                "url": "http://consumernotebook.com/grids/audreyr/womens-wallets-styled-like-mens-wallets/",
                "username": "audreyr"
            },
            {
                "id": "4f49baf5feac66000d000005",
                "last_modified_by_user": "2012-02-25T21:00:52.055000",
                "resource_uri": "/api/v1/grids/4f49baf5feac66000d000005/",
                "slug": "padded-double-compartment-laptop-bags-for-2-laptops",
                "title": "Padded Double Compartment Laptop Bags (for 2 laptops)",
                "url": "http://consumernotebook.com/grids/audreyr/padded-double-compartment-laptop-bags-for-2-laptops/",
                "username": "audreyr"
            }
        ]
    }