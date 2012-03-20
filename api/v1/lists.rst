.. _api-v1-lists:

=====================
GET /api/v1/lists/
=====================

Returns the most recent lists added to Consumer Notebook.  This method is can only return up to 20 lists at a time.

Parameters
==========

access_token
    Oauth2 access token required for all Consumer Notebook REST API requests.

format (optional)
    * json (default)
    * jsonp
    
offset (optional)
    Specifies the page of results to retrieve. Defaults to 0.

Example Request
================

Get::

    curl https://consumernotebook.com/api/v1/lists/ -d access_token={access_token} -G
    
Results:    

.. sourcecode:: javascript

    {
        "meta": {
            "limit": 20,
            "next": "/api/v1/lists/?access_token={access_token}&limit=20&offset=20",
            "offset": 0,
            "previous": null,
            "total_count": 242
        },
        "objects": [{
            "created": "2012-03-18T15:26:41.179900",
            "description": "Laptops specifically designed to run Linux. These either a) come with some flavor of Linux installed, or b) come with Windows and have no or minimal driver issues when you install Linux.  Note: this list is a work in progress.",
            "id": "536",
            "last_modified_by_user": "2012-03-18T15:42:12.241595",
            "modified": "2012-03-18T15:42:12.268523",
            "owner": {
                "avatar": "https://consumernotebook.s3.amazonaws.com/avatars/audreyr/resized/80/avatars/audreyr/audreyr.jpg",
                "coins": 149,
                "fullname": "Audrey M. Roy",
                "score": 1029,
                "username": "audreyr",
                "waitlisted": false
            },
            "products": [{
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//zareason.com/shop/Alto-3880.html",
                "comment": "$649+. 14\" HD (1366x768), 5 hr battery life, 4.5 lbs.",
                "id": "4f6661219007d7000c000000",
                "image_url": "http://zareason.com/shop/images/P/front%20300.png",
                "price_range": "$500-1000",
                "resource_url": "/api/v1/products/4f6661219007d7000c000000/",
                "title": "ZaReason Alto 3880"
            },
            {
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//zareason.com/shop/Strata-6770.html",
                "comment": "$849. 15.6\" HD (1366x768), Second Generation Core Processor, Nvidia 540m 1gb",
                "id": "4f66622d9007d7000e000004",
                "image_url": "http://zareason.com/shop/images/P/Front%20top%20300%20no%20background.png",
                "price_range": "$500-1000",
                "resource_url": "/api/v1/products/4f66622d9007d7000e000004/",
                "title": "ZaReason Strata 6770"
            },
            {
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//zareason.com/shop/Verix-17.html",
                "comment": "$1499. 17\" HD (1920x1080), Hyper-threaded CPU provides up to 8 threads of processing power to rival desktop processing power.",
                "id": "4f6662ff9007d7000e000006",
                "image_url": "http://zareason.com/shop/images/P/verix17300.png",
                "price_range": "$1000-2000",
                "resource_url": "/api/v1/products/4f6662ff9007d7000e000006/",
                "title": "ZaReason Verix 17"
            },
            {
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//zareason.com/shop/Chimera.html",
                "comment": "$2299. \"The ultimate, most powerful, and most widely functional\" laptop made for Linux, according to the ZaReason website.",
                "id": "4f6663809007d7000d000003",
                "image_url": "http://zareason.com/shop/images/P/chimera300-01.png",
                "price_range": "$2000-5000",
                "resource_url": "/api/v1/products/4f6663809007d7000d000003/",
                "title": "ZaReason Chimera"
            },
            {
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//zareason.com/shop/Verix-2.5.html",
                "comment": "$1799. HD 1080p 15.6\" and good balance between power and affordability.",
                "id": "4f6663e39007d7000c000002",
                "image_url": "http://zareason.com/shop/images/P/Verix_300.png",
                "price_range": "$1000-2000",
                "resource_url": "/api/v1/products/4f6663e39007d7000c000002/",
                "title": "ZaReason Verix 2.5"
            },
            {
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=https%3A//www.system76.com/laptops/model/lemur",
                "comment": "$639. \"Ultra Portable, Ultra Powerful.\" 4.71 lbs. ",
                "id": "4f66649a9007d7000e000008",
                "image_url": "https://www.system76.com/product_images/lemur-177a7b0ff967a0b.png",
                "price_range": "$500-1000",
                "resource_url": "/api/v1/products/4f66649a9007d7000e000008/",
                "title": "14.1\" Lemur Ultra by System76"
            }],
            "resource_uri": "/api/v1/lists/536/",
            "slug": "linux-laptops",
            "title": "Linux Laptops"
        },
        {
            "created": "2012-03-17T12:08:40.179512",
            "description": "",
            "id": "535",
            "last_modified_by_user": "2012-03-16T22:06:03.535662",
            "modified": "2012-03-17T21:32:25.721127",
            "owner": {
                "avatar": "https://consumernotebook.s3.amazonaws.com/avatars/jaredahardy/resized/80/avatars/jaredahardy/jaredahardy.jpg",
                "coins": 0,
                "fullname": "Jared Hardy",
                "score": 3,
                "username": "jaredahardy",
                "waitlisted": false
            },
            "products": [{
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.popsci.com/gadgets/gallery/2012-02/goods-march-2012s-hottest-gadgets%3Fimage%3D4",
                "comment": "",
                "id": "4f64e138555803000e000009",
                "image_url": "http://www.popsci.com/files/imagecache/photogallery_image/articles/PSC0312_WN_095.jpg",
                "price_range": "$50-100",
                "resource_url": "/api/v1/products/4f64e138555803000e000009/",
                "title": "Planetary Gears Corkscrew"
            }],
            "resource_uri": "/api/v1/lists/535/",
            "slug": "kitchen",
            "title": "Kitchen"
        },
        {
            "created": "2012-03-17T11:24:36.808447",
            "description": "",
            "id": "534",
            "last_modified_by_user": "2012-03-16T22:06:03.535662",
            "modified": "2012-03-17T21:32:25.738290",
            "owner": {
                "avatar": "https://consumernotebook.s3.amazonaws.com/avatars/frogmonkey/resized/80/avatars/frogmonkey/frogmonkey.jpg",
                "coins": 10,
                "fullname": "Johnny Cheng",
                "score": 9,
                "username": "frogmonkey",
                "waitlisted": false
            },
            "products": [{
                "affiliate_link": "http://www.amazon.com/gp/product/B003Y3BJ7S/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "",
                "id": "4f64d7ad555803000e000005",
                "image_url": "http://ecx.images-amazon.com/images/I/51g762U2t8L.jpg",
                "price_range": "$100-200",
                "resource_url": "/api/v1/products/4f64d7ad555803000e000005/",
                "title": "Viewsonic VX2450WM-LED 24-Inch (23.6-Inch Vis) Widescreen LED Monitor with Full HD 1080p and Speaker"
            }],
            "resource_uri": "/api/v1/lists/534/",
            "slug": "monitors-24",
            "title": "Monitors -24\""
        },
        {
            "created": "2012-03-09T21:14:50.456887",
            "description": "",
            "id": "533",
            "last_modified_by_user": "2012-03-09T17:53:46.275580",
            "modified": "2012-03-17T21:32:25.770861",
            "owner": {
                "avatar": "https://consumernotebook.s3.amazonaws.com/avatars/regebro/resized/80/avatars/regebro/regebro.jpg",
                "coins": 30,
                "fullname": "Lennart Regebro",
                "score": 30,
                "username": "regebro",
                "waitlisted": false
            },
            "products": [{
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.domyos-fitness.com/EN/ve-200-silver-200934556/",
                "comment": "",
                "id": "4f5ae34a36a633000c000000",
                "image_url": "http://www.domyos-fitness.com/products-pictures/400/asset_76930445.jpg",
                "price_range": "Free",
                "resource_url": "/api/v1/products/4f5ae34a36a633000c000000/",
                "title": "Domyos - VE 200 SILVER - Elliptical machines - - Designed for \u00a0occasional cardio-training at home"
            },
            {
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.domyos-fitness.com/EN/ve410-192417016/",
                "comment": "",
                "id": "4f5ae3b736a633000d000002",
                "image_url": "http://www.domyos-fitness.com/products-pictures/400/asset_48312560.jpg",
                "price_range": "$100-200",
                "resource_url": "/api/v1/products/4f5ae3b736a633000d000002/",
                "title": "Domyos - VE410 - Elliptical machines - - Designed for \u00a0occasional to regular cardio-training at home"
            },
            {
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.domyos-fitness.com/EN/ve410-limited-192434670/",
                "comment": "",
                "id": "4f5ae5351cfd5d000d000002",
                "image_url": "http://www.domyos-fitness.com/EN/images/assets/100228-logo.jpg",
                "price_range": "$100-200",
                "resource_url": "/api/v1/products/4f5ae5351cfd5d000d000002/",
                "title": "Domyos - VE410 Limited - Elliptical machines - - Designed for \u00a0occasional to REGULAR\u00a0cardio-training"
            },
            {
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.domyos-fitness.com/EN/ve510-192434399/%23infoPlusTab",
                "comment": "",
                "id": "4f5ae7e91cfd5d000d000004",
                "image_url": "http://www.domyos-fitness.com/EN/images/assets/100228-logo.jpg",
                "price_range": "$200-500",
                "resource_url": "/api/v1/products/4f5ae7e91cfd5d000d000004/",
                "title": "Domyos - VE510 - Elliptical machines - - Designed for \u00a0occasional to REGULAR\u00a0cardio-training at home"
            },
            {
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.decathlon.com.pl/PL/ve710-192894659/",
                "comment": "",
                "id": "4f5ae8621cfd5d000d000006",
                "image_url": "http://www.decathlon.com.pl/products-pictures/250/gd-asset_71010738.jpg",
                "price_range": "$500-1000",
                "resource_url": "/api/v1/products/4f5ae8621cfd5d000d000006/",
                "title": "DOMYOS - VE710 elliptical trainer for home use"
            },
            {
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.decathlon.com.pl/PL/e7zl-135420218/",
                "comment": "",
                "id": "4f5ae99036a633000c000002",
                "image_url": "http://www.decathlon.com.pl/products-pictures/250/gd-asset_36134608.jpg",
                "price_range": "$500-1000",
                "resource_url": "/api/v1/products/4f5ae99036a633000c000002/",
                "title": "NordicTrack E 4.0 Elliptical trainer"
            },
            {
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//esklep.intersport.pl/pl/product/60438/crosstrainer-energetics-power-et-7.5-163035",
                "comment": "",
                "id": "4f5c706fc83e70000d000000",
                "image_url": "http://esklep.intersport.pl/images/products/zoom/10-WIOSNA-ENERGETICS-163035_1436586879043987800_1287574412.jpg",
                "price_range": "$200-500",
                "resource_url": "/api/v1/products/4f5c706fc83e70000d000000/",
                "title": "Energetics Power ET 7.5"
            },
            {
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//esklep.intersport.pl/pl/product/60242/crosstrainer-energetics-magnetic-et-5.5-163028",
                "comment": "",
                "id": "4f5c709ac83e70000d000002",
                "image_url": "http://esklep.intersport.pl/images/products/zoom/10-WIOSNA-ENERGETICS-163028_981509187009678100_1287391267.jpg",
                "price_range": "$200-500",
                "resource_url": "/api/v1/products/4f5c709ac83e70000d000002/",
                "title": "Energetics Magnetic ET 5.5"
            }],
            "resource_uri": "/api/v1/lists/533/",
            "slug": "elliptical-trainers",
            "title": "Elliptical trainers"
        },
        {
            "created": "2012-03-08T22:17:42.952447",
            "description": "",
            "id": "532",
            "last_modified_by_user": "2012-03-08T17:07:56.810606",
            "modified": "2012-03-17T21:32:25.795121",
            "owner": {
                "avatar": "/media/avatars/pydanny/resized/80/avatars/pydanny/daniel.greenfeld.jpg",
                "coins": 122,
                "fullname": "Daniel Greenfeld",
                "score": 695,
                "username": "pydanny",
                "waitlisted": false
            },
            "products": [{
                "affiliate_link": "http://www.amazon.com/gp/product/B0053BG370/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "",
                "id": "4f59a086204d33000e000000",
                "image_url": "http://ecx.images-amazon.com/images/I/61fezndpqNL.jpg",
                "price_range": "$50-100",
                "resource_url": "/api/v1/products/4f59a086204d33000e000000/",
                "title": "MotionSports Adrenaline: XBox"
            },
            {
                "affiliate_link": "http://www.amazon.com/gp/product/B004U9T6FM/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "A super heroku fight game? Sign me up!",
                "id": "4f59a0f55ddae9000d000000",
                "image_url": "http://ecx.images-amazon.com/images/I/61j1tcm6ZjL.jpg",
                "price_range": "$20-50",
                "resource_url": "/api/v1/products/4f59a0f55ddae9000d000000/",
                "title": "PowerUP Heroes: XBox"
            },
            {
                "affiliate_link": "http://www.amazon.com/gp/product/B002I0H8FK/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "I like games",
                "id": "4f5b9c9f24b4b3000e000003",
                "image_url": "http://ecx.images-amazon.com/images/I/5109BtpAZPL.jpg",
                "price_range": "$20-50",
                "resource_url": "/api/v1/products/4f5b9c9f24b4b3000e000003/",
                "title": "Child Of Eden: Xbox 360: Video Games"
            },
            {
                "affiliate_link": "http://www.amazon.com/gp/product/B0056WJA3K/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "deepak!",
                "id": "4f5b9e1736a633000d000006",
                "image_url": "http://ecx.images-amazon.com/images/I/51llqktiEZL.jpg",
                "price_range": "$20-50",
                "resource_url": "/api/v1/products/4f5b9e1736a633000d000006/",
                "title": "Deepak Chopra's Leela: Xbox 360: Video Games"
            },
            {
                "affiliate_link": "http://www.amazon.com/gp/product/B00061NL7W/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "Dance!",
                "id": "4f5ba47936a633000e000006",
                "image_url": "http://ecx.images-amazon.com/images/I/51vm-es1RUL.jpg",
                "price_range": "$50-100",
                "resource_url": "/api/v1/products/4f5ba47936a633000e000006/",
                "title": "Yourself Fitness: Xbox:"
            },
            {
                "affiliate_link": "http://www.amazon.com/gp/product/B002I0H9WM/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "guy is punching!",
                "id": "4f5bab081cfd5d000c000008",
                "image_url": "http://ecx.images-amazon.com/images/I/51gcyDU9V%2BL.jpg",
                "price_range": "$50-100",
                "resource_url": "/api/v1/products/4f5bab081cfd5d000c000008/",
                "title": "Your Shape Fitness Evolved: Video Games"
            }],
            "resource_uri": "/api/v1/lists/532/",
            "slug": "kinect-games",
            "title": "Kinect Games"
        },
        {
            "created": "2012-03-06T22:45:07.526120",
            "description": "These are the best Apple accessories I've found. If you're fully invested in Apple products, you may want to bookmark this. Let me know if I've missed anything.",
            "id": "531",
            "last_modified_by_user": "2012-03-06T22:51:05.250910",
            "modified": "2012-03-17T21:32:25.814521",
            "owner": {
                "avatar": "https://consumernotebook.s3.amazonaws.com/avatars/audreyr/resized/80/avatars/audreyr/audreyr.jpg",
                "coins": 149,
                "fullname": "Audrey M. Roy",
                "score": 1029,
                "username": "audreyr",
                "waitlisted": false
            },
            "products": [{
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//lightake.com/detail.do/sku.Ultrathin_Bluetooth_Slide_Out_Wireless_Keyboard_Hard_Case_for_iPhone_4_Black_-42711",
                "comment": "The worst thing about the iPhone 4 is having to type on the hard glass screen. This slide-out keyboard makes typing quicker and less painful.",
                "id": "4f5703f37709ac000e000000",
                "image_url": "http://img.lightake.com/image201102/sku_42711_1.JPG",
                "price_range": "$20-50",
                "resource_url": "/api/v1/products/4f5703f37709ac000e000000/",
                "title": "Ultrathin Bluetooth Slide-Out Wireless Keyboard Hard Case for iPhone 4 Black"
            },
            {
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//lightake.com/detail.do/sku.Yosion_Apple_Peel_520_Turns_iPod_Touch_into_an_iPhone_Black-32674",
                "comment": "It's kind of crazy that you can even do this.",
                "id": "4f5704ad7709ac000c000000",
                "image_url": "http://www.lightake.com/uploadImg/2010101417163546.JPG",
                "price_range": "$20-50",
                "resource_url": "/api/v1/products/4f5704ad7709ac000c000000/",
                "title": "Yosion Apple Peel 520 Turns iPod Touch into an iPhone Black"
            },
            {
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//ibottleopener.myshopify.com/products/ibottleopener-4",
                "comment": "You can open beer bottles with this hardshell iPhone case.",
                "id": "4f580f60e75dbc000c000000",
                "image_url": "http://cdn.shopify.com/s/files/1/0079/3682/products/5_large.jpg?1004",
                "price_range": "$10-20",
                "resource_url": "/api/v1/products/4f580f60e75dbc000c000000/",
                "title": "iBottleopener for iPhone 4/4s"
            }],
            "resource_uri": "/api/v1/lists/531/",
            "slug": "best-apple-accessories",
            "title": "Best Apple Accessories"
        },
        {
            "created": "2012-03-06T17:18:52.312598",
            "description": "",
            "id": "530",
            "last_modified_by_user": "2012-03-06T17:07:08.617723",
            "modified": "2012-03-17T21:32:25.843404",
            "owner": {
                "avatar": "/media/avatars/pydanny/resized/80/avatars/pydanny/daniel.greenfeld.jpg",
                "coins": 122,
                "fullname": "Daniel Greenfeld",
                "score": 695,
                "username": "pydanny",
                "waitlisted": false
            },
            "products": [{
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.magazinediscountcenter.com/magazine-subscription/Discover.html",
                "comment": "Discover is a good mix of articles over a wide range of subjects. Also, it's website is served out with the Python programming language.",
                "id": "4f56b77cda8e7c000c000000",
                "image_url": "http://www.magazinediscountcenter.com/images/prod_images/large/363.jpg",
                "price_range": "$20-50",
                "resource_url": "/api/v1/products/4f56b77cda8e7c000c000000/",
                "title": "Discover Magazine"
            },
            {
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.magazinediscountcenter.com/magazine-subscription/Science-Illustrated.html",
                "comment": "Sue me, I love the pretty space pictures in this magazine. No matter how good monitors get, you can't get the same thing electronically.",
                "id": "4f56b7ccdd779f000d000000",
                "image_url": "http://www.magazinediscountcenter.com/images/prod_images/large/800.jpg",
                "price_range": "$20-50",
                "resource_url": "/api/v1/products/4f56b7ccdd779f000d000000/",
                "title": "Science Illustrated Magazine"
            },
            {
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.magazinediscountcenter.com/magazine-subscription/Scientific-American.html",
                "comment": "I started reading this recently thanks to my electrician. While waiting ro the inspector, he had a few in his van. ",
                "id": "4f56b857dd779f000d000002",
                "image_url": "http://www.magazinediscountcenter.com/images/prod_images/large/714.jpg",
                "price_range": "$20-50",
                "resource_url": "/api/v1/products/4f56b857dd779f000d000002/",
                "title": "Scientific American Magazine"
            }],
            "resource_uri": "/api/v1/lists/530/",
            "slug": "magazines-i-should-read",
            "title": "Magazines I should read"
        },
        {
            "created": "2012-03-06T07:31:43.429811",
            "description": "",
            "id": "529",
            "last_modified_by_user": "2012-03-06T06:52:07.526073",
            "modified": "2012-03-17T21:32:25.862315",
            "owner": {
                "avatar": "https://consumernotebook.s3.amazonaws.com/avatars/audreyr/resized/80/avatars/audreyr/audreyr.jpg",
                "coins": 149,
                "fullname": "Audrey M. Roy",
                "score": 1029,
                "username": "audreyr",
                "waitlisted": false
            },
            "products": [{
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.sharperimage.com/si/view/product/iPad-Wireless-Keyboard-Case/200436%3Ftrail%3D",
                "comment": "",
                "id": "4f562ddf6d58bc000c000000",
                "image_url": "http://www.sharperimage.com/dyn/dyn/MEDIA_CustomProductCatalog/m680954_200436-iPad-Type-Case-P1.jpg",
                "price_range": "$50-100",
                "resource_url": "/api/v1/products/4f562ddf6d58bc000c000000/",
                "title": "iPad Wireless Keyboard Case"
            },
            {
                "affiliate_link": "http://www.amazon.com/gp/product/B007BVJZ0C/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "Not a kindle two accessory, just doing this to show it off.",
                "id": "4f5a99ce310cb0000e000004",
                "image_url": "http://ecx.images-amazon.com/images/I/51sCEBmPE4L.jpg",
                "price_range": "Free",
                "resource_url": "/api/v1/products/4f5a99ce310cb0000e000004/",
                "title": "Game of Thrones [HD]: Season 1, Episode 0 \"Making Game of Thrones [HD]\": Amazon Instant Video"
            }],
            "resource_uri": "/api/v1/lists/529/",
            "slug": "most-useful-ipad-ipad-2-accessories",
            "title": "Most Useful iPad / iPad 2 Accessories"
        },
        {
            "created": "2012-03-06T04:08:41.636537",
            "description": "A variety of stuff I own, which I've neglected due to old age or...I just don't like it any more.",
            "id": "528",
            "last_modified_by_user": "2012-03-09T03:46:57.211269",
            "modified": "2012-03-17T21:32:25.882831",
            "owner": {
                "avatar": "https://consumernotebook.s3.amazonaws.com/avatars/knockycode/resized/80/avatars/knockycode/knockycode.png",
                "coins": 40,
                "fullname": "Jenny Key Nguyen",
                "score": 55,
                "username": "knockycode",
                "waitlisted": false
            },
            "products": [{
                "affiliate_link": "http://www.amazon.com/gp/product/B00005B8G2/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "My first ever Nintendo console purchase. I was late to the game.",
                "id": "4f3c0163ebae26000400003a",
                "image_url": "http://ecx.images-amazon.com/images/I/51a%2BjB8bahL.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f3c0163ebae26000400003a/",
                "title": "Nintendo Game Boy Advance - White"
            },
            {
                "affiliate_link": "http://www.amazon.com/gp/product/B000MXF2IK/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "This was a birthday gift. I've been using it for two years and it still works perfectly fine. I've dropped it a few times too. My cousin, who has dropped his a dozen of times, can still use it despite it being quite battered-looking.",
                "id": "4f3c016bebae2600040000bf",
                "image_url": "http://ecx.images-amazon.com/images/I/41rvjzCoMlL.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f3c016bebae2600040000bf/",
                "title": "Nokia 6300 Unlocked Triband Camera Business Phone (Black)"
            },
            {
                "affiliate_link": "http://www.amazon.com/gp/product/B0002TW8A4/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "Beware. I did not get my Feiyue shoes from Amazon. I only really use these shoes either for daily use or for parkour. They offer too much grip for martial arts, making moves such as sliding and shifting stances quickly on wooden flooring incredibly difficult. Also, the pair I have are starting to fall apart with just half a year of mostly daily use. I most probably got a bad pair, because my fellow traceurs (who got theirs from the same chain) kept theirs in good condition even after several months of much heavier training.",
                "id": "4f3c019cebae260004000194",
                "image_url": "http://ecx.images-amazon.com/images/I/41eHC6B2UjL.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f3c019cebae260004000194/",
                "title": "Black Feiyue Martial Arts Shoes - Size 45"
            },
            {
                "affiliate_link": "http://www.amazon.com/gp/product/B000084313/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "Another Pokemon game I have. Have replayed this a few times, but won't in the future. The newer versions are more entertaining than this one. They have better Pokemon choices too.",
                "id": "4f3c01a4ebae26000400021e",
                "image_url": "http://ecx.images-amazon.com/images/I/618K8K3FZGL.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f3c01a4ebae26000400021e/",
                "title": "Pokemon Ruby"
            }],
            "resource_uri": "/api/v1/lists/528/",
            "slug": "knockycodes-neglected-possessions",
            "title": "Knockycode's Neglected Possessions"
        },
        {
            "created": "2012-03-06T04:01:47.965406",
            "description": "A variety of stuff I want. :)",
            "id": "527",
            "last_modified_by_user": "2012-03-12T04:57:19.581620",
            "modified": "2012-03-17T21:32:25.909886",
            "owner": {
                "avatar": "https://consumernotebook.s3.amazonaws.com/avatars/knockycode/resized/80/avatars/knockycode/knockycode.png",
                "coins": 40,
                "fullname": "Jenny Key Nguyen",
                "score": 55,
                "username": "knockycode",
                "waitlisted": false
            },
            "products": [{
                "affiliate_link": "http://www.amazon.com/gp/product/B0050SVMYA/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "One of my two DS Lite systems is dying. And there are a couple of games I want to play that is only on the 3DS.",
                "id": "4f3c0169ebae260004000079",
                "image_url": "http://ecx.images-amazon.com/images/I/41VfRkANkYL.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f3c0169ebae260004000079/",
                "title": "Nintendo 3DS - Flame Red"
            },
            {
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.thinkgeek.com/tshirts-apparel/hoodies/8cd1/",
                "comment": "I love hoodies. And it'd be nice to wear this, if enough people bug me about fixing their computers.",
                "id": "4f55fd8ff4ee1c000d000000",
                "image_url": "http://www.thinkgeek.com/images/products/frontsquare/fix_your_computer_hoodie.jpg",
                "price_range": "$20-50",
                "resource_url": "/api/v1/products/4f55fd8ff4ee1c000d000000/",
                "title": "ThinkGeek :: No I will not fix your computer Hoodie"
            },
            {
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.thinkgeek.com/tshirts-apparel/unisex/itdepartment/e95e/%3Fcpg%3D162H%26image",
                "comment": "Gotta love shirts. And I love the line on this one.",
                "id": "4f55ff04ceca95000d000002",
                "image_url": "http://www.thinkgeek.com/images/products/frontsquare/e95e_telnet_mordor.jpg",
                "price_range": "$10-20",
                "resource_url": "/api/v1/products/4f55ff04ceca95000d000002/",
                "title": "ThinkGeek :: One Does Not Simply Telnet into Mordor"
            },
            {
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//headphones.com.au/psingle%3FproductID%3D509",
                "comment": "Looks light to wear for long periods of time, and its mic is apparently compatible with iOS and Android phones.",
                "id": "4f560025fba307000d000000",
                "image_url": "http://www.headphones.com.au/images/prods/aiaiai/tracks.jpg",
                "price_range": "$50-100",
                "resource_url": "/api/v1/products/4f560025fba307000d000000/",
                "title": "Aiaiai: Tracks"
            },
            {
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=https%3A//shop.androidacademy.com/accessories/cozybot-green.html",
                "comment": "A phone holder would be nice when I need the phone to act as a camera or video recorder.",
                "id": "4f58ce2f23d31e000e000000",
                "image_url": "https://shop.androidacademy.com/media/catalog/product/cache/1/image/265x265/9df78eab33525d08d6e5fb8d27136e95/6/4/640x480-01.jpg",
                "price_range": "$0-10",
                "resource_url": "/api/v1/products/4f58ce2f23d31e000e000000/",
                "title": "CozyBot (Green) - Accessories"
            }],
            "resource_uri": "/api/v1/lists/527/",
            "slug": "knockycodes-wishlist",
            "title": "Knockycode's Wishlist"
        },
        {
            "created": "2012-03-05T16:36:09.413737",
            "description": "Various sources I've found for heirloom seeds.",
            "id": "526",
            "last_modified_by_user": "2012-03-05T17:31:05.296844",
            "modified": "2012-03-17T21:32:25.939106",
            "owner": {
                "avatar": "https://consumernotebook.s3.amazonaws.com/avatars/audreyr/resized/80/avatars/audreyr/audreyr.jpg",
                "coins": 149,
                "fullname": "Audrey M. Roy",
                "score": 1029,
                "username": "audreyr",
                "waitlisted": false
            },
            "products": [{
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.non-hybrid-seeds.com/sp/specialty-packs/tomato-lover-s-pack-59.html",
                "comment": "",
                "id": "4f555bf9682343000d000000",
                "image_url": "http://www.non-hybrid-seeds.com/sp/media/catalog/product/cache/1/image/9df78eab33525d08d6e5fb8d27136e95/t/o/tom-icon-lg.jpg",
                "price_range": "$20-50",
                "resource_url": "/api/v1/products/4f555bf9682343000d000000/",
                "title": "12 Variety Heirloom Tomato Seed Pack"
            },
            {
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.non-hybrid-seeds.com/sp/specialty-packs/tea-garden-69.html",
                "comment": "Grow 21 different varieties of tea, including black and green tea.",
                "id": "4f563bac2a588b000e000000",
                "image_url": "http://www.non-hybrid-seeds.com/sp/media/catalog/product/cache/1/image/9df78eab33525d08d6e5fb8d27136e95/t/e/tea-icon-lg.jpg",
                "price_range": "$50-100",
                "resource_url": "/api/v1/products/4f563bac2a588b000e000000/",
                "title": "Herbal Tea Garden Seeds from Heirloom Organics"
            }],
            "resource_uri": "/api/v1/lists/526/",
            "slug": "heirloom-fruit-vegetable-and-herb-gardening",
            "title": "Heirloom Fruit, Vegetable, and Herb Gardening"
        },
        {
            "created": "2012-03-05T15:35:55.857935",
            "description": "Kits for home-brewing or making traditionally store-bought gourmet food items at home.",
            "id": "525",
            "last_modified_by_user": "2012-03-05T15:57:17.652039",
            "modified": "2012-03-17T21:32:25.967714",
            "owner": {
                "avatar": "https://consumernotebook.s3.amazonaws.com/avatars/audreyr/resized/80/avatars/audreyr/audreyr.jpg",
                "coins": 149,
                "fullname": "Audrey M. Roy",
                "score": 1029,
                "username": "audreyr",
                "waitlisted": false
            },
            "products": [{
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.mexgrocer.com/14990.html",
                "comment": "A kit for making your own tamales. Includes hard-to-find masa, corn husks, a tamale steamer, and more.",
                "id": "4f554bcb4037ea000d000000",
                "image_url": "http://pics.mexgrocer.com/images/14990.jpg",
                "price_range": "$20-50",
                "resource_url": "/api/v1/products/4f554bcb4037ea000d000000/",
                "title": "Mexican Tamale Lovers Gift Pack - 5 Items"
            },
            {
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.fudgekitchen.co.uk/home-kit/",
                "comment": "Includes mixes for plain, chocolate, and toffee fudges, plus all the tools and instructions you need to make foolproof fudge at home.  All you need to add is cream.",
                "id": "4f554ddbd769fa000e000000",
                "image_url": "http://www.fudgekitchen.co.uk/images/images/new%20make%20at%20home.jpg",
                "price_range": "Free",
                "resource_url": "/api/v1/products/4f554ddbd769fa000e000000/",
                "title": "Make Fudge at Home Kit, from Fudge Kitchen"
            },
            {
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.mightyleaf.com/matcha-green-tea/green-tea-latte-set/",
                "comment": "Make coffee shop style green tea lattes at home.",
                "id": "4f554f4d52f06c000c000000",
                "image_url": "http://www.mightyleaf.com/resources/mightyleaf/images/products/processed/Green_Tea_Latte_Set.a.detail.jpg",
                "price_range": "$50-100",
                "resource_url": "/api/v1/products/4f554f4d52f06c000c000000/",
                "title": "Green Tea Latte Set in Loose Tea Matcha, Mighty Leaf"
            },
            {
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.mrbeer.com/category-exec/category_id/189",
                "comment": "Makes 2 gallons of root beer in as little as 3 days. Includes everything, even the bottles.",
                "id": "4f55518dd769fa000d000000",
                "image_url": "http://www.mrbeer.com/images/products/86-LRG.jpg",
                "price_range": "$20-50",
                "resource_url": "/api/v1/products/4f55518dd769fa000d000000/",
                "title": "Mr. Root Beer Kit"
            },
            {
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.mrbeer.com/category-exec/category_id/186",
                "comment": "Make fermented hard cider at home.",
                "id": "4f555215d769fa000d000002",
                "image_url": "http://www.mrbeer.com/images/products/519-LRG.jpg",
                "price_range": "$50-100",
                "resource_url": "/api/v1/products/4f555215d769fa000d000002/",
                "title": "Mr.Beer Archer's Orchard Hard Cider Kit"
            },
            {
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.mrbeer.com/category-exec/category_id/249",
                "comment": "Makes 2 batches of home-brewed beer.",
                "id": "4f55528f52f06c000d000002",
                "image_url": "http://www.mrbeer.com/images/products/933b-LRG.jpg",
                "price_range": "$50-100",
                "resource_url": "/api/v1/products/4f55528f52f06c000d000002/",
                "title": "Mr.Beer Premium Edition Extra Beer Kit"
            }],
            "resource_uri": "/api/v1/lists/525/",
            "slug": "diy-foodie-kits",
            "title": "DIY Foodie Kits"
        },
        {
            "created": "2012-03-05T12:57:49.696813",
            "description": "List of resources for Scrum",
            "id": "524",
            "last_modified_by_user": "2012-03-05T09:29:54.425210",
            "modified": "2012-03-17T21:32:25.986197",
            "owner": {
                "avatar": "https://consumernotebook.s3.amazonaws.com/avatars/paulhildebrandt/resized/80/avatars/paulhildebrandt/Profile.jpg",
                "coins": 0,
                "fullname": "Paul Hildebrandt",
                "score": 4,
                "username": "paulhildebrandt",
                "waitlisted": false
            },
            "products": [{
                "affiliate_link": "http://www.amazon.com/gp/product/B004IDNS6S/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "Good Product Owner book",
                "id": "4f5528644fa437000d000000",
                "image_url": null,
                "price_range": "$50-100",
                "resource_url": "/api/v1/products/4f5528644fa437000d000000/",
                "title": "A Book of Five Rings: The Strategy of Musashi (Audible Audio Edition)"
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
            "modified": "2012-03-17T21:32:26.014847",
            "owner": {
                "avatar": "/media/avatars/pydanny/resized/80/avatars/pydanny/daniel.greenfeld.jpg",
                "coins": 122,
                "fullname": "Daniel Greenfeld",
                "score": 695,
                "username": "pydanny",
                "waitlisted": false
            },
            "products": [{
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.magazinediscountcenter.com/magazine-subscription/Cooking-Light.html",
                "comment": "My mom stays really healthy through good eating of lighter foods. This is an awesome periodical to help her out.",
                "id": "4f5439c1ba376c000c000000",
                "image_url": "https://consumernotebook.s3.amazonaws.com/products/www.magazinediscountcenter.com/images/prod_images/large/331.jpg",
                "price_range": "$20-50",
                "resource_url": "/api/v1/products/4f5439c1ba376c000c000000/",
                "title": "Cooking Light Magazine"
            },
            {
                "affiliate_link": "http://www.amazon.com/gp/product/B002IYHIKG/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "This is great for any garden, large or small. Mom can pack in a lot of herbs or flowers into a small location in a very attractive package.",
                "id": "4f5453dfb15ef7000e000000",
                "image_url": "http://ecx.images-amazon.com/images/I/41%2Bz99pmfVL.jpg",
                "price_range": "$20-50",
                "resource_url": "/api/v1/products/4f5453dfb15ef7000e000000/",
                "title": "Akro-Mils Stack-A-Pot"
            },
            {
                "affiliate_link": "http://www.amazon.com/gp/product/B004TN51EE/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "Yoga has been taken up by a lot of active, retired moms. This mat stays odor free pretty much forever, and is thick enough to keep joints off cold, hard floors.",
                "id": "4f54546cb15ef7000e000002",
                "image_url": "http://ecx.images-amazon.com/images/I/41i3G25PRZL.jpg",
                "price_range": "$20-50",
                "resource_url": "/api/v1/products/4f54546cb15ef7000e000002/",
                "title": "Aurorae Classic Yoga Mat - Always smells good."
            },
            {
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.flowersacrossamerica.com/product.cfm%3Fdcode%3DC26-2943",
                "comment": "Because of their longevity, moms often prefer plants over flowers. ",
                "id": "4f5459dfb15ef7000c000006",
                "image_url": "http://www.flowersacrossamerica.com/flowers/products/C26-2943.jpg",
                "price_range": "$50-100",
                "resource_url": "/api/v1/products/4f5459dfb15ef7000c000006/",
                "title": "French Garden - Best Selling Flowers"
            },
            {
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.newegg.com/Product/Product.aspx%3FItem%3DN82E16834230171",
                "comment": "On the pricey side of things, this ultrabook has the grace of the MacBook Air and the familiarity of Windows.",
                "id": "4f545c01b15ef7000c000008",
                "image_url": "http://images17.newegg.com/is/image/newegg/34-230-171-TS?$S300W$",
                "price_range": "$1000-2000",
                "resource_url": "/api/v1/products/4f545c01b15ef7000c000008/",
                "title": "ASUS Zenbook UX31E-DH52 Ultrabook i5 1.70GHz 13.3\" 4GB  128GB SSD HDD"
            },
            {
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.newegg.com/Product/Product.aspx%3FItem%3DN82E16834230359",
                "comment": "A nicely affordable laptop to give your mom, the Asus brand is known for their quality components and assembly.",
                "id": "4f545ceeb15ef7000e000004",
                "image_url": "http://images10.newegg.com/NeweggImage/ProductImageCompressAll300/34-230-359-02.jpg",
                "price_range": "$200-500",
                "resource_url": "/api/v1/products/4f545ceeb15ef7000e000004/",
                "title": "ASUS Eee PC Matte Black Intel Atom N2600, 1.60GHz 10.1\" 1GB DDR3 Memory 320GB HDD Netbook"
            },
            {
                "affiliate_link": "http://www.amazon.com/gp/product/B00166DR9S/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "She types a lot.",
                "id": "4f5a7c07204d33000c000001",
                "image_url": "http://ecx.images-amazon.com/images/I/4158fFJJcUL.jpg",
                "price_range": "$100-200",
                "resource_url": "/api/v1/products/4f5a7c07204d33000c000001/",
                "title": "Boss Black LeatherPlus Executive Chair"
            }],
            "resource_uri": "/api/v1/lists/523/",
            "slug": "gifts-to-give-your-retired-mom",
            "title": "Gifts to give your retired mom"
        },
        {
            "created": "2012-03-04T19:56:57.185368",
            "description": "Creative, thoughtful gift ideas for family members whom you love dearly but are hard to buy for.",
            "id": "522",
            "last_modified_by_user": "2012-03-05T14:52:41.358025",
            "modified": "2012-03-17T21:32:26.050164",
            "owner": {
                "avatar": "https://consumernotebook.s3.amazonaws.com/avatars/audreyr/resized/80/avatars/audreyr/audreyr.jpg",
                "coins": 149,
                "fullname": "Audrey M. Roy",
                "score": 1029,
                "username": "audreyr",
                "waitlisted": false
            },
            "products": [{
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.magazinediscountcenter.com/magazine-subscription/Budget-Travel.html",
                "comment": "For the person who loves to travel and experience new things every year.",
                "id": "4f54398912c882000e000000",
                "image_url": "https://consumernotebook.s3.amazonaws.com/products/www.magazinediscountcenter.com/images/prod_images/large/278.jpg",
                "price_range": "$20-50",
                "resource_url": "/api/v1/products/4f54398912c882000e000000/",
                "title": "Budget Travel Magazine"
            },
            {
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.magazinediscountcenter.com/magazine-subscription/Cooking-Light.html",
                "comment": "A thoughtful gift for the person who loves cooking, but not the gourmet full-fat kind of cooking.",
                "id": "4f5439c1ba376c000c000000",
                "image_url": "https://consumernotebook.s3.amazonaws.com/products/www.magazinediscountcenter.com/images/prod_images/large/331.jpg",
                "price_range": "$20-50",
                "resource_url": "/api/v1/products/4f5439c1ba376c000c000000/",
                "title": "Cooking Light Magazine"
            },
            {
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.uncommongoods.com/product/growbottle",
                "comment": "An easy-to-grow hydroponic tabletop herb garden. Available in basil, chive, mint, oregano, or parsley.",
                "id": "4f5543274fa437000c000003",
                "image_url": "http://data.uncommongoods.com.edgesuite.net/images/newweb/product/20169_zoom3.jpg",
                "price_range": "$20-50",
                "resource_url": "/api/v1/products/4f5543274fa437000c000003/",
                "title": "GROWBOTTLE Indoor Herb Garden Kit"
            },
            {
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.target.com/p/Twill-French-Memo-Board-Ivory-17x20/-/A-10635957%23%3Flnk%3Dsc_qi_detaillink",
                "comment": "Anyone who likes saving ticket stubs and printing photos would appreciate this.",
                "id": "4f55464d8524f8000d000003",
                "image_url": "http://img2.targetimg2.com/wcsstore/TargetSAS//img/p/10/63/10635957.jpg",
                "price_range": "$10-20",
                "resource_url": "/api/v1/products/4f55464d8524f8000d000003/",
                "title": "Twill French Memo Board"
            },
            {
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.target.com/p/Norelco-7340/-/A-11034504%23%3Flnk%3Dsc_qi_detailbutton",
                "comment": "A useful gift for teenage boys and young men.",
                "id": "4f5546f58524f8000e000002",
                "image_url": "http://img3.targetimg3.com/wcsstore/TargetSAS//img/p/11/03/11034504.jpg",
                "price_range": "$20-50",
                "resource_url": "/api/v1/products/4f5546f58524f8000e000002/",
                "title": "Norelco 7340"
            },
            {
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.target.com/p/ELF-Never-Too-Much-Palette-144-Piece/-/A-13716713%23%3Flnk%3Dsc_qi_detaillink",
                "comment": "Young women who are just getting into makeup would appreciate a huge makeup color palette like this.",
                "id": "4f55481f8524f8000d000005",
                "image_url": "http://img2.targetimg2.com/wcsstore/TargetSAS//img/p/13/71/13716713.jpg",
                "price_range": "$10-20",
                "resource_url": "/api/v1/products/4f55481f8524f8000d000005/",
                "title": "ELF Never Too Much Palette - 144 Piece"
            },
            {
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.target.com/p/Chefmate-Pizza-Stone/-/A-13770560%23%3Flnk%3Dsc_qi_detaillink",
                "comment": "A pizza stone that can be put on the gas grill or into the oven. A fun idea for those who can't cook except on the grill.",
                "id": "4f55492cc79bd1000e000000",
                "image_url": "http://img3.targetimg3.com/wcsstore/TargetSAS//img/p/13/77/13770560.jpg",
                "price_range": "$20-50",
                "resource_url": "/api/v1/products/4f55492cc79bd1000e000000/",
                "title": "Chefmate Pizza Stone"
            },
            {
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.mexgrocer.com/14990.html",
                "comment": "For the ethnic gourmet chef. Comes with hard-to-find items like corn husks and a tamale steamer pot.",
                "id": "4f554bcb4037ea000d000000",
                "image_url": "http://pics.mexgrocer.com/images/14990.jpg",
                "price_range": "$20-50",
                "resource_url": "/api/v1/products/4f554bcb4037ea000d000000/",
                "title": "Mexican Tamale Lovers Gift Pack - 5 Items"
            },
            {
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.cheryls.com/new%21-happy-birthday-tin--treats-assortment.product.701822.90010",
                "comment": "A tin filled with gorgeous assorted cookies. It plays the \"Happy Birthday\" song when you open it. For $5 extra, you can add a mini chocolate cake with candles too.",
                "id": "4f554d294037ea000e000000",
                "image_url": "http://a248.e.akamai.net/f/764/16447/1h/www.cheryls.com/wcsstore/CherylAndCompany/images/catalog/SJH69801z.jpg",
                "price_range": "$20-50",
                "resource_url": "/api/v1/products/4f554d294037ea000e000000/",
                "title": "Musical Happy Birthday Tin of Treats, from Cheryl's"
            },
            {
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.mightyleaf.com/gifts_gift-boxes/herbal-tea-master-tea-pouch-sampler/",
                "comment": "This assortment of 108 Tea Pouches includes 18 pouches each of Organic African Nectar, Organic Mint Melange, Organic Detox Infusion, Chamomile Citrus, Ginger Twist, and Rainforest Mat\u00e9.",
                "id": "4f554facd769fa000c000000",
                "image_url": "http://www.mightyleaf.com/resources/mightyleaf/images/products/processed/35504.a.detail.jpg",
                "price_range": "$20-50",
                "resource_url": "/api/v1/products/4f554facd769fa000c000000/",
                "title": "Herbal Tea Master Tea Pouch Sampler, from Mighty Leaf"
            },
            {
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.kmart.com/shc/s/p_10151_10104_479000000DT3795PP%3FprdNo%3D8%26blockNo%3D8%26blockType%3DG8",
                "comment": "For the woman who loves to garden.",
                "id": "4f562700d5913d000c000000",
                "image_url": "http://s.shld.net/is/image/Sears/479000000DT3795P?hei=315&wid=315&op_sharpen=1&resMode=sharp&op_usm=0.9,0.5,0,0",
                "price_range": "$50-100",
                "resource_url": "/api/v1/products/4f562700d5913d000c000000/",
                "title": "Apollo 18 Piece Garden Tool Kit, Pink"
            },
            {
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.sharperimage.com/si/view/product/iPhone-Photo-Cube-Printer/200196%3Ftrail%3D",
                "comment": "Lets you print iPhone photos directly, without a computer or even a connector cable.",
                "id": "4f562d706d58bc000d000000",
                "image_url": "http://www.sharperimage.com/dyn/dyn/MEDIA_CustomProductCatalog/m490035_200196-p2.jpg",
                "price_range": "$100-200",
                "resource_url": "/api/v1/products/4f562d706d58bc000d000000/",
                "title": "iPhone Photo Cube Printer"
            }],
            "resource_uri": "/api/v1/lists/522/",
            "slug": "gift-ideas-for-family",
            "title": "Gift Ideas For Family"
        },
        {
            "created": "2012-03-04T18:39:04.811248",
            "description": "What you need in your basic disaster preparedness kit, adapted from ready.gov/basic-disaster-supplies-kit.",
            "id": "521",
            "last_modified_by_user": "2012-03-04T18:43:52.026523",
            "modified": "2012-03-17T21:32:26.092433",
            "owner": {
                "avatar": "https://consumernotebook.s3.amazonaws.com/avatars/audreyr/resized/80/avatars/audreyr/audreyr.jpg",
                "coins": 149,
                "fullname": "Audrey M. Roy",
                "score": 1029,
                "username": "audreyr",
                "waitlisted": false
            },
            "products": [{
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.sparkletts.com/shopping/large-bottles.jsf",
                "comment": "You need 1 gallon of water per day per person, for at least 3 days.  For drinking and sanitation.",
                "id": "4f54274829566a000c000000",
                "image_url": "https://consumernotebook.s3.amazonaws.com/products/www.sparkletts.com/images/large-bottles/sparkletts-5-gallon-spring.jpg",
                "price_range": "$100-200",
                "resource_url": "/api/v1/products/4f54274829566a000c000000/",
                "title": "Monthly Water Delivery Plan from water.com"
            },
            {
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.efoodsdirect.com/store/index.php/shop/responders/7-day-responder.html",
                "comment": "You need at least a 3-day supply of non-perishable food. The eFoods Direct food box provides one adult with 44 servings and is rated well compared with other emergency food brands.",
                "id": "4f5429094a0f9c000d000000",
                "image_url": "https://consumernotebook.s3.amazonaws.com/products/www.efoodsdirect.com/store/media/catalog/product/cache/1/image/375x/9df78eab33525d08d6e5fb8d27136e95/1/_/1_week_responder.jpg",
                "price_range": "$50-100",
                "resource_url": "/api/v1/products/4f5429094a0f9c000d000000/",
                "title": "7-Day Responder Emergency Meals"
            },
            {
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.target.com/p/Discovery-Expedition-Self-Powered-AM-FM-SW-NOAA-Weather-Radio-Silver-D105X/-/A-13375246",
                "comment": "A battery-powered or hand crank radio and a NOAA Weather Radio with tone alert are recommended. This serves as both and can be powered by battery, hand-crank, solar, or traditional electricity.",
                "id": "4f542b75d7781e000d000000",
                "image_url": "https://consumernotebook.s3.amazonaws.com/products/img3.targetimg3.com/wcsstore/TargetSAS/img/p/13/37/13375246.jpg",
                "price_range": "$50-100",
                "resource_url": "/api/v1/products/4f542b75d7781e000d000000/",
                "title": "Discovery Expedition Self-Powered AM/FM/SW/NOAA Weather Radio"
            },
            {
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.target.com/p/Energizer-Max-AA-Alkaline-Batteries-24-ct/-/A-13738866",
                "comment": "Extra batteries for the radio.",
                "id": "4f542c914a0f9c000d000002",
                "image_url": "https://consumernotebook.s3.amazonaws.com/products/img1.targetimg1.com/wcsstore/TargetSAS/img/p/13/73/13738866.jpg",
                "price_range": "$10-20",
                "resource_url": "/api/v1/products/4f542c914a0f9c000d000002/",
                "title": "Energizer Max AA Alkaline Batteries 24-ct."
            },
            {
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.target.com/p/Life-Gear-Glow-400-hr-Flashlight-Assorted-Colors/-/A-12916890",
                "comment": "A long-life flashlight. This one is waterproof and floats if dropped in water.",
                "id": "4f54435499b9ed000d000000",
                "image_url": "https://consumernotebook.s3.amazonaws.com/products/img2.targetimg2.com/wcsstore/TargetSAS/img/p/12/91/12916890.jpg",
                "price_range": "$0-10",
                "resource_url": "/api/v1/products/4f54435499b9ed000d000000/",
                "title": "Life Gear Glow 400-hr. Flashlight"
            },
            {
                "affiliate_link": "http://www.amazon.com/gp/product/B0007CL02S/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "A second heavy-duty flashlight. The built-in cell phone charger is a must-have, so that you can reach family/friends in an emergency.",
                "id": "4f5444bfb15ef7000c000000",
                "image_url": "http://ecx.images-amazon.com/images/I/41xGSABAGJL.jpg",
                "price_range": "$20-50",
                "resource_url": "/api/v1/products/4f5444bfb15ef7000c000000/",
                "title": "Solar / Hand-Crank Powered Emergency Flashlight, Radio, & Cell Phone Charger"
            },
            {
                "affiliate_link": "http://www.amazon.com/gp/product/B0043X5WK8/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "Obviously, a first aid kit is critical for emergencies. This one is reasonably priced and gets top reviews, plus it's the only kit that comes with Save-A-Tooth.",
                "id": "4f544c77ce806b000d000000",
                "image_url": "http://ecx.images-amazon.com/images/I/41JbDrxiGZL.jpg",
                "price_range": "$20-50",
                "resource_url": "/api/v1/products/4f544c77ce806b000d000000/",
                "title": "The Complete First Aid Kit - Includes Save-A-Tooth, Exceeds ANSI Standards"
            },
            {
                "affiliate_link": "http://www.amazon.com/gp/product/B002YK4U2I/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "Don't forget first aid for your pets.",
                "id": "4f544d61ce806b000e000000",
                "image_url": "http://ecx.images-amazon.com/images/I/51Hq5HAeb8L.jpg",
                "price_range": "$10-20",
                "resource_url": "/api/v1/products/4f544d61ce806b000e000000/",
                "title": "AKC 20-Piece Pet First Aid Kit"
            },
            {
                "affiliate_link": "http://www.amazon.com/gp/product/B001H8FJIW/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "Being able to call for help in a disaster with a loud whistle can save your life. Reviewers rated this one as one of the loudest at a distance.",
                "id": "4f544f25653614000c000000",
                "image_url": "http://ecx.images-amazon.com/images/I/31jEw07yFDL.jpg",
                "price_range": "$20-50",
                "resource_url": "/api/v1/products/4f544f25653614000c000000/",
                "title": "Storm Safety Whistle"
            },
            {
                "affiliate_link": "http://www.amazon.com/gp/product/B0002YKBV2/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "During or after a natural disaster, you may need to protect your lungs with a dust mask. These are inexpensive and allow better air flow than the non-respirator version.",
                "id": "4f545256ce806b000c000000",
                "image_url": "http://ecx.images-amazon.com/images/I/31bFcqAaf-L.jpg",
                "price_range": "$10-20",
                "resource_url": "/api/v1/products/4f545256ce806b000c000000/",
                "title": "3M 8511 Particulate Sanding Respirator N95 with Valve, 10-Pack"
            },
            {
                "affiliate_link": "http://www.amazon.com/gp/product/B0014UH8XW/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "Plastic sheeting in case you need to shelter in place due to airborne contaminants. It sounds crazy, but it's part of the kit recommended by ready.gov and the EPA.",
                "id": "4f5454b8653614000d000000",
                "image_url": "http://ecx.images-amazon.com/images/I/21whKU-y4ZL.jpg",
                "price_range": "$20-50",
                "resource_url": "/api/v1/products/4f5454b8653614000d000000/",
                "title": "Clear Plastic Poly Sheeting 10' x 100' 6 mil"
            },
            {
                "affiliate_link": "http://www.amazon.com/gp/product/B002KQ6682/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "Duct tape to hold up the plastic sheeting.",
                "id": "4f5454f6ce806b000d000002",
                "image_url": "http://ecx.images-amazon.com/images/I/51PSTHbMnBL.jpg",
                "price_range": "$10-20",
                "resource_url": "/api/v1/products/4f5454f6ce806b000d000002/",
                "title": "Intertape 5038-3 PK Fix-It DUCTape 1.87-Inches x 60-Yards, 7-Mil, 3-Pack"
            },
            {
                "affiliate_link": "http://www.amazon.com/gp/product/B000FZ23FA/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "Moist towelettes for personal sanitation. Individually-wrapped ones like these help reduce the risk of contamination.",
                "id": "4f545581b15ef7000c000002",
                "image_url": "http://ecx.images-amazon.com/images/I/510%2BQonCNgL.jpg",
                "price_range": "$0-10",
                "resource_url": "/api/v1/products/4f545581b15ef7000c000002/",
                "title": "PURELL Sanitizing Hand Wipes Individually Wrapped 100-ct. Box"
            },
            {
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.target.com/p/Glad-Large-Trash-Bags-30-Gallon-30-Count/-/A-13022830%23%3Flnk%3Dsc_qi_detaillink",
                "comment": "Heavy-duty drawstring garbage bags, for personal sanitation.",
                "id": "4f545657653614000c000002",
                "image_url": "http://img3.targetimg3.com/wcsstore/TargetSAS//img/p/13/02/13022830.jpg",
                "price_range": "$0-10",
                "resource_url": "/api/v1/products/4f545657653614000c000002/",
                "title": "Glad Large Trash Bags 30 Gallon 30 Count"
            },
            {
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.homedepot.com/h_d1/N-5yc1v/R-100002119/h_d2/ProductDisplay%3FcatalogId%3D10053%26langId%3D-1%26keyword%3Dpliers%26storeId%3D10051",
                "comment": "A wrench or pliers for turning off the utilities.",
                "id": "4f5456ecce806b000e000002",
                "image_url": "http://www.homedepot.com/catalog/productImages/300/13/13c8e441-c54f-4cd6-975c-fcf329ee90ae_300.jpg",
                "price_range": "$10-20",
                "resource_url": "/api/v1/products/4f5456ecce806b000e000002/",
                "title": "Channellock 12 In. Tongue and Groove Pliers"
            },
            {
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.target.com/p/Zyliss-Lock-and-Lift-Can-Opener-White/-/A-10513110%23%3Flnk%3Dsc_qi_detaillink",
                "comment": "A manual can opener for food. This one is around $15; reviewers say it's more durable than other can openers. You don't want your can opener to break in an emergency.",
                "id": "4f5457fa653614000e000000",
                "image_url": "http://img3.targetimg3.com/wcsstore/TargetSAS//img/p/10/51/10513110.jpg",
                "price_range": "$10-20",
                "resource_url": "/api/v1/products/4f5457fa653614000e000000/",
                "title": "Zyliss Lock-and-Lift Can Opener"
            },
            {
                "affiliate_link": "http://www.amazon.com/gp/product/0528870467/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "You may need to get to an unfamiliar evacuation center when a disaster occurs. You won't be able to look up directions online when the power goes out.",
                "id": "4f5458a3b15ef7000c000004",
                "image_url": "http://ecx.images-amazon.com/images/I/41E-r11nQ-L.jpg",
                "price_range": "$10-20",
                "resource_url": "/api/v1/products/4f5458a3b15ef7000c000004/",
                "title": "Thomas Guide Los Angeles County, 63rd Edition"
            }],
            "resource_uri": "/api/v1/lists/521/",
            "slug": "basic-emergency-supply-list",
            "title": "Basic Emergency Supply List"
        },
        {
            "created": "2012-03-04T17:21:03.642119",
            "description": "",
            "id": "520",
            "last_modified_by_user": "2012-03-04T15:07:21.424985",
            "modified": "2012-03-17T21:32:26.112345",
            "owner": {
                "avatar": "https://consumernotebook.s3.amazonaws.com/avatars/paulhildebrandt/resized/80/avatars/paulhildebrandt/Profile.jpg",
                "coins": 0,
                "fullname": "Paul Hildebrandt",
                "score": 4,
                "username": "paulhildebrandt",
                "waitlisted": false
            },
            "products": [{
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//propertyware.com/",
                "comment": "",
                "id": "4f5414ff29566a000e000000",
                "image_url": "https://consumernotebook.s3.amazonaws.com/products/www.propertyware.com/images/banner_logo.png",
                "price_range": "Free",
                "resource_url": "/api/v1/products/4f5414ff29566a000e000000/",
                "title": "Online Property Management "
            }],
            "resource_uri": "/api/v1/lists/520/",
            "slug": "property-management",
            "title": "Property Management"
        },
        {
            "created": "2012-02-29T18:51:23.108433",
            "description": "",
            "id": "519",
            "last_modified_by_user": "2012-02-29T18:19:48.453489",
            "modified": "2012-03-17T21:32:26.137972",
            "owner": {
                "avatar": "https://consumernotebook.s3.amazonaws.com/avatars/shawnr/resized/80/avatars/shawnr/shawnr.jpg",
                "coins": 10,
                "fullname": "Shawn Rider",
                "score": 10,
                "username": "shawnr",
                "waitlisted": false
            },
            "products": [{
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//us.playstation.com/psvita/games-and-media/psv-touch-my-katamari.html",
                "comment": "This is the first worthy handheld version of the franchise.",
                "id": "4f4ee42b9b8acf000e000000",
                "image_url": "https://consumernotebook.s3.amazonaws.com/products/webassetsi.scea.com/pscomauth/groups/public/documents/webasset/psv-tm-katamari-packfront.jpg",
                "price_range": "$20-50",
                "resource_url": "/api/v1/products/4f4ee42b9b8acf000e000000/",
                "title": "Touch my Katamari"
            },
            {
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//us.playstation.com/psvita/games-and-media/psv-escape-plan.html",
                "comment": "This is a PSN downloadable puzzle game with a quirky aesthetic that makes use of all the input methods of the PS Vita.",
                "id": "4f4ee4c5a8e53a000c000001",
                "image_url": "https://consumernotebook.s3.amazonaws.com/products/webassetsf.scea.com/pscomauth/groups/public/documents/webasset/psv-escape-plan-packfront.jpg",
                "price_range": "$10-20",
                "resource_url": "/api/v1/products/4f4ee4c5a8e53a000c000001/",
                "title": "Escape Plan"
            },
            {
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//us.playstation.com/psvita/games-and-media/psv-dungeon-hunter-alliance.html",
                "comment": "An excellent dungeon-crawler RPG with multiplayer co-op support. The evolution of the iOS franchise, too.",
                "id": "4f4ee525a8e53a000e000001",
                "image_url": "https://consumernotebook.s3.amazonaws.com/products/webassetsc.scea.com/pscomauth/groups/public/documents/webasset/psv-dungeon-hunter-packfront.jpg",
                "price_range": "Free",
                "resource_url": "/api/v1/products/4f4ee525a8e53a000e000001/",
                "title": "Dungeon Hunter Alliance"
            },
            {
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//us.playstation.com/psvita/games-and-media/psv-dynasty-warriors.html",
                "comment": "The best of the Dynasty Warriors franchise so far, this deserves a shot (especially since there is a free demo).",
                "id": "4f4ee6149b8acf000c000000",
                "image_url": "https://consumernotebook.s3.amazonaws.com/products/webassetsd.scea.com/pscomauth/groups/public/documents/webasset/psv-dyn-warr-nxt-packfront.jpg",
                "price_range": "Free",
                "resource_url": "/api/v1/products/4f4ee6149b8acf000c000000/",
                "title": "DYNASTY WARRIORS NEXT"
            },
            {
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//us.playstation.com/psvita/games-and-media/psv-uncharted-golden-abyss.html",
                "comment": "This installment of the Uncharted series probably tries too hard to show off all the new input mechanisms of the PS Vita, but it is just as good as the PS3 games.",
                "id": "4f4ee66c9b8acf000e000002",
                "image_url": "https://consumernotebook.s3.amazonaws.com/products/webassetsh.scea.com/pscomauth/groups/public/documents/webasset/e32011-game-5517-packfront.jpg",
                "price_range": "$20-50",
                "resource_url": "/api/v1/products/4f4ee66c9b8acf000e000002/",
                "title": "Uncharted: Golden Abyss"
            },
            {
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//us.playstation.com/psvita/games-and-media/psv-rayman-origins.html",
                "comment": "Excellent graphics, a great sense of humor, and solid gameplay make this another quality installment of this 2D platformer series.",
                "id": "4f4ee6ada8e53a000d000000",
                "image_url": "https://consumernotebook.s3.amazonaws.com/products/webassetsj.scea.com/pscomauth/groups/public/documents/webasset/psv-rayman-orig-packfront.jpg",
                "price_range": "$20-50",
                "resource_url": "/api/v1/products/4f4ee6ada8e53a000d000000/",
                "title": "Rayman Origins"
            },
            {
                "affiliate_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//us.playstation.com/psvita/games-and-media/psv-modnation-racers.html",
                "comment": "Kooky cart racing optimized for online multiplayer.",
                "id": "4f4ee6e1405f62000e000000",
                "image_url": "https://consumernotebook.s3.amazonaws.com/products/webassetsh.scea.com/pscomauth/groups/public/documents/webasset/psv-mod-racers-packfront.jpg",
                "price_range": "$20-50",
                "resource_url": "/api/v1/products/4f4ee6e1405f62000e000000/",
                "title": "ModNation Racers"
            }],
            "resource_uri": "/api/v1/lists/519/",
            "slug": "ps-vita-games-i-have-played",
            "title": "PS Vita Games I Have Played"
        },
        {
            "created": "2012-02-29T13:32:17.209313",
            "description": "",
            "id": "518",
            "last_modified_by_user": "2012-02-28T17:44:00.994009",
            "modified": "2012-03-17T21:32:26.154919",
            "owner": {
                "avatar": "https://consumernotebook.s3.amazonaws.com/avatars/mark0978/resized/80/avatars/mark0978/mark0978.JPG",
                "coins": 0,
                "fullname": "Mark Jones",
                "score": 2,
                "username": "mark0978",
                "waitlisted": false
            },
            "products": [],
            "resource_uri": "/api/v1/lists/518/",
            "slug": "and-what-is-the-list-for",
            "title": "And what is the list for?"
        },
        {
            "created": "2012-02-28T12:27:49.398490",
            "description": "",
            "id": "517",
            "last_modified_by_user": "2012-02-28T10:13:31.720443",
            "modified": "2012-03-17T21:32:26.172434",
            "owner": {
                "avatar": "https://consumernotebook.s3.amazonaws.com/avatars/saevarom/resized/80/avatars/saevarom/saevarom.jpeg",
                "coins": 10,
                "fullname": "S\u00e6var \u00d6fj\u00f6r\u00f0 Magn\u00fasson",
                "score": 5,
                "username": "saevarom",
                "waitlisted": false
            },
            "products": [{
                "affiliate_link": "http://www.amazon.com/gp/product/B0000YWF5E/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "",
                "id": "4f4d38f5e46e7c000c000003",
                "image_url": "http://ecx.images-amazon.com/images/I/31Y8KvCGpUL.jpg",
                "price_range": "$20-50",
                "resource_url": "/api/v1/products/4f4d38f5e46e7c000c000003/",
                "title": "Chemex Drip Coffee Carafe - 6 Cup: Amazon.com: Kitchen & Dining"
            },
            {
                "affiliate_link": "http://www.amazon.com/gp/product/B0043EWFAM/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "",
                "id": "4f4d3918fbf36a000c000001",
                "image_url": "http://ecx.images-amazon.com/images/I/415sT7qPpeL.jpg",
                "price_range": "$100-200",
                "resource_url": "/api/v1/products/4f4d3918fbf36a000c000001/",
                "title": "Breville BCG800XL Smart Grinder"
            },
            {
                "affiliate_link": "http://www.amazon.com/gp/product/B0000CF3HB/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "",
                "id": "4f4d393b0b00be000c000002",
                "image_url": "http://ecx.images-amazon.com/images/I/41Lg8D9VFaL.jpg",
                "price_range": "$20-50",
                "resource_url": "/api/v1/products/4f4d393b0b00be000c000002/",
                "title": "Chemex Coffee Filters - 100 Chemex Bonded Unbleached Filter Squares FSU-100"
            },
            {
                "affiliate_link": "http://www.amazon.com/gp/product/B0000CFKTO/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "",
                "id": "4f4d396cfbf36a000d000003",
                "image_url": "http://ecx.images-amazon.com/images/I/21RVEJ8N4QL.jpg",
                "price_range": "$0-10",
                "resource_url": "/api/v1/products/4f4d396cfbf36a000d000003/",
                "title": "Chemex Glass Coffeemaker Lid: Amazon.com"
            }],
            "resource_uri": "/api/v1/lists/517/",
            "slug": "coffee-gear",
            "title": "Coffee gear"
        }]
    }