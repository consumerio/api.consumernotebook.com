.. _api-v1-my-lists:

=======================
GET /api/v1/my-lists/
=======================

Returns your lists.

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

    curl https://consumernotebook.com/api/v1/my-lists/ -d access_token={access_token} -G
    
Results:    

.. sourcecode:: javascript

    {
        "meta": {
            "limit": 20,
            "next": "/api/v1/my-lists/?access_token={access_token}&limit=20&offset=20",
            "offset": 0,
            "previous": null,
            "total_count": 26
        },
        "objects": [{
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
                "external_link": "http://www.amazon.com/gp/product/B0053BG370/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "",
                "id": "4f59a086204d33000e000000",
                "image_url": "http://ecx.images-amazon.com/images/I/61fezndpqNL.jpg",
                "price_range": "$50-100",
                "resource_url": "/api/v1/products/4f59a086204d33000e000000/",
                "title": "MotionSports Adrenaline: XBox"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/B004U9T6FM/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "A super heroku fight game? Sign me up!",
                "id": "4f59a0f55ddae9000d000000",
                "image_url": "http://ecx.images-amazon.com/images/I/61j1tcm6ZjL.jpg",
                "price_range": "$20-50",
                "resource_url": "/api/v1/products/4f59a0f55ddae9000d000000/",
                "title": "PowerUP Heroes: XBox"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/B002I0H8FK/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "I like games",
                "id": "4f5b9c9f24b4b3000e000003",
                "image_url": "http://ecx.images-amazon.com/images/I/5109BtpAZPL.jpg",
                "price_range": "$20-50",
                "resource_url": "/api/v1/products/4f5b9c9f24b4b3000e000003/",
                "title": "Child Of Eden: Xbox 360: Video Games"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/B0056WJA3K/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "deepak!",
                "id": "4f5b9e1736a633000d000006",
                "image_url": "http://ecx.images-amazon.com/images/I/51llqktiEZL.jpg",
                "price_range": "$20-50",
                "resource_url": "/api/v1/products/4f5b9e1736a633000d000006/",
                "title": "Deepak Chopra's Leela: Xbox 360: Video Games"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/B00061NL7W/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "Dance!",
                "id": "4f5ba47936a633000e000006",
                "image_url": "http://ecx.images-amazon.com/images/I/51vm-es1RUL.jpg",
                "price_range": "$50-100",
                "resource_url": "/api/v1/products/4f5ba47936a633000e000006/",
                "title": "Yourself Fitness: Xbox:"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/B002I0H9WM/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "guy is punching!",
                "id": "4f5bab081cfd5d000c000008",
                "image_url": "http://ecx.images-amazon.com/images/I/51gcyDU9V%2BL.jpg",
                "price_range": "$50-100",
                "resource_url": "/api/v1/products/4f5bab081cfd5d000c000008/",
                "title": "Your Shape Fitness Evolved: Video Games"
            }],
            "resource_uri": "/api/v1/my-lists/532/",
            "slug": "kinect-games",
            "title": "Kinect Games"
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
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.magazinediscountcenter.com/magazine-subscription/Discover.html",
                "comment": "Discover is a good mix of articles over a wide range of subjects. Also, it's website is served out with the Python programming language.",
                "id": "4f56b77cda8e7c000c000000",
                "image_url": "http://www.magazinediscountcenter.com/images/prod_images/large/363.jpg",
                "price_range": "$20-50",
                "resource_url": "/api/v1/products/4f56b77cda8e7c000c000000/",
                "title": "Discover Magazine"
            },
            {
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.magazinediscountcenter.com/magazine-subscription/Science-Illustrated.html",
                "comment": "Sue me, I love the pretty space pictures in this magazine. No matter how good monitors get, you can't get the same thing electronically.",
                "id": "4f56b7ccdd779f000d000000",
                "image_url": "http://www.magazinediscountcenter.com/images/prod_images/large/800.jpg",
                "price_range": "$20-50",
                "resource_url": "/api/v1/products/4f56b7ccdd779f000d000000/",
                "title": "Science Illustrated Magazine"
            },
            {
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.magazinediscountcenter.com/magazine-subscription/Scientific-American.html",
                "comment": "I started reading this recently thanks to my electrician. While waiting ro the inspector, he had a few in his van. ",
                "id": "4f56b857dd779f000d000002",
                "image_url": "http://www.magazinediscountcenter.com/images/prod_images/large/714.jpg",
                "price_range": "$20-50",
                "resource_url": "/api/v1/products/4f56b857dd779f000d000002/",
                "title": "Scientific American Magazine"
            }],
            "resource_uri": "/api/v1/my-lists/530/",
            "slug": "magazines-i-should-read",
            "title": "Magazines I should read"
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
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.magazinediscountcenter.com/magazine-subscription/Cooking-Light.html",
                "comment": "My mom stays really healthy through good eating of lighter foods. This is an awesome periodical to help her out.",
                "id": "4f5439c1ba376c000c000000",
                "image_url": "https://consumernotebook.s3.amazonaws.com/products/www.magazinediscountcenter.com/images/prod_images/large/331.jpg",
                "price_range": "$20-50",
                "resource_url": "/api/v1/products/4f5439c1ba376c000c000000/",
                "title": "Cooking Light Magazine"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/B002IYHIKG/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "This is great for any garden, large or small. Mom can pack in a lot of herbs or flowers into a small location in a very attractive package.",
                "id": "4f5453dfb15ef7000e000000",
                "image_url": "http://ecx.images-amazon.com/images/I/41%2Bz99pmfVL.jpg",
                "price_range": "$20-50",
                "resource_url": "/api/v1/products/4f5453dfb15ef7000e000000/",
                "title": "Akro-Mils Stack-A-Pot"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/B004TN51EE/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "Yoga has been taken up by a lot of active, retired moms. This mat stays odor free pretty much forever, and is thick enough to keep joints off cold, hard floors.",
                "id": "4f54546cb15ef7000e000002",
                "image_url": "http://ecx.images-amazon.com/images/I/41i3G25PRZL.jpg",
                "price_range": "$20-50",
                "resource_url": "/api/v1/products/4f54546cb15ef7000e000002/",
                "title": "Aurorae Classic Yoga Mat - Always smells good."
            },
            {
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.flowersacrossamerica.com/product.cfm%3Fdcode%3DC26-2943",
                "comment": "Because of their longevity, moms often prefer plants over flowers. ",
                "id": "4f5459dfb15ef7000c000006",
                "image_url": "http://www.flowersacrossamerica.com/flowers/products/C26-2943.jpg",
                "price_range": "$50-100",
                "resource_url": "/api/v1/products/4f5459dfb15ef7000c000006/",
                "title": "French Garden - Best Selling Flowers"
            },
            {
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.newegg.com/Product/Product.aspx%3FItem%3DN82E16834230171",
                "comment": "On the pricey side of things, this ultrabook has the grace of the MacBook Air and the familiarity of Windows.",
                "id": "4f545c01b15ef7000c000008",
                "image_url": "http://images17.newegg.com/is/image/newegg/34-230-171-TS?$S300W$",
                "price_range": "$1000-2000",
                "resource_url": "/api/v1/products/4f545c01b15ef7000c000008/",
                "title": "ASUS Zenbook UX31E-DH52 Ultrabook i5 1.70GHz 13.3\" 4GB  128GB SSD HDD"
            },
            {
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.newegg.com/Product/Product.aspx%3FItem%3DN82E16834230359",
                "comment": "A nicely affordable laptop to give your mom, the Asus brand is known for their quality components and assembly.",
                "id": "4f545ceeb15ef7000e000004",
                "image_url": "http://images10.newegg.com/NeweggImage/ProductImageCompressAll300/34-230-359-02.jpg",
                "price_range": "$200-500",
                "resource_url": "/api/v1/products/4f545ceeb15ef7000e000004/",
                "title": "ASUS Eee PC Matte Black Intel Atom N2600, 1.60GHz 10.1\" 1GB DDR3 Memory 320GB HDD Netbook"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/B00166DR9S/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "She types a lot.",
                "id": "4f5a7c07204d33000c000001",
                "image_url": "http://ecx.images-amazon.com/images/I/4158fFJJcUL.jpg",
                "price_range": "$100-200",
                "resource_url": "/api/v1/products/4f5a7c07204d33000c000001/",
                "title": "Boss Black LeatherPlus Executive Chair"
            }],
            "resource_uri": "/api/v1/my-lists/523/",
            "slug": "gifts-to-give-your-retired-mom",
            "title": "Gifts to give your retired mom"
        },
        {
            "created": "2012-02-26T16:57:07.354140",
            "description": "Help me fill this out. Send me recommendations to my twitter account as pydanny.",
            "id": "503",
            "last_modified_by_user": "2012-02-27T09:41:07.737663",
            "modified": "2012-03-17T21:32:26.540636",
            "owner": {
                "avatar": "/media/avatars/pydanny/resized/80/avatars/pydanny/daniel.greenfeld.jpg",
                "coins": 122,
                "fullname": "Daniel Greenfeld",
                "score": 695,
                "username": "pydanny",
                "waitlisted": false
            },
            "products": [{
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//macromates.com/",
                "comment": "",
                "id": "4f4ad4e35a4305000d000000",
                "image_url": "https://consumernotebook.s3.amazonaws.com/products/manual.macromates.com/images/project_window_with_tabs.png",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f4ad4e35a4305000d000000/",
                "title": "TextMate: The Missing Editor for Mac OS X"
            },
            {
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.sublimetext.com/",
                "comment": "",
                "id": "4f4ad53a5a4305000e000000",
                "image_url": "https://consumernotebook.s3.amazonaws.com/products/www.sublimetext.com/screenshots/pythonHeroSmall.png",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f4ad53a5a4305000e000000/",
                "title": "Sublime Text"
            },
            {
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.jetbrains.com/pycharm/index.html",
                "comment": "",
                "id": "4f4ad5b861e9e4000e000000",
                "image_url": "https://consumernotebook.s3.amazonaws.com/products/www.jetbrains.com/img/logo_bw.gif",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f4ad5b861e9e4000e000000/",
                "title": "JetBrains PyCharm"
            },
            {
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//pydev.org/",
                "comment": "",
                "id": "4f4ad5d55a4c6f000d000000",
                "image_url": "https://consumernotebook.s3.amazonaws.com/products/pydev.org/images/pydev_banner2.gif",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f4ad5d55a4c6f000d000000/",
                "title": "PyDev"
            },
            {
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=https%3A//store.activestate.com/komodo-ide",
                "comment": "",
                "id": "4f4bedc7776e5e000c000000",
                "image_url": "https://consumernotebook.s3.amazonaws.com/products/store.activestate.com/sites/default/files/category_pictures/box_2012_komodo_ide_7.png",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f4bedc7776e5e000c000000/",
                "title": "Komodo IDE 7 from ActiveState"
            },
            {
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.microsoftstore.com/store/msstore/en_US/pd/productID.216633300/topseller.true",
                "comment": "According to codeplex, VS supports both Iron Python and CPython.",
                "id": "4f4c298b611f84000d000000",
                "image_url": "https://consumernotebook.s3.amazonaws.com/products/dri1.img.digitalrivercontent.net/DRHM/Storefront/Company/msstore/images/software/pdp/en-US_Visual_Studio_Pro_2010_ESD_C5E-00532.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f4c298b611f84000d000000/",
                "title": "Microsoft Visual Studio 2010 Professional"
            }],
            "resource_uri": "/api/v1/my-lists/503/",
            "slug": "complete-list-of-python-editors",
            "title": "Complete List of Python Editors"
        },
        {
            "created": "2012-02-25T13:24:39.212716",
            "description": "",
            "id": "500",
            "last_modified_by_user": "2012-02-25T11:59:07.083030",
            "modified": "2012-03-17T21:32:26.616569",
            "owner": {
                "avatar": "/media/avatars/pydanny/resized/80/avatars/pydanny/daniel.greenfeld.jpg",
                "coins": 122,
                "fullname": "Daniel Greenfeld",
                "score": 695,
                "username": "pydanny",
                "waitlisted": false
            },
            "products": [{
                "external_link": "http://www.amazon.com/gp/product/B0050SW8OS/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "",
                "id": "4f4951976721be000e000002",
                "image_url": "http://ecx.images-amazon.com/images/I/51%2Bqo7LzBgL.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f4951976721be000e000002/",
                "title": "Uncharted: Golden Abyss"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/B006PP41Q8/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "",
                "id": "4f4951ac3ad8f20012000000",
                "image_url": "http://ecx.images-amazon.com/images/I/31lvjvwfwxL.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f4951ac3ad8f20012000000/",
                "title": "PlayStation Vita Travel Pouch"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/B006WJ6YH6/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "",
                "id": "4f4951bcdd83af000d000000",
                "image_url": "http://ecx.images-amazon.com/images/I/61UdIS4QRTL.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f4951bcdd83af000d000000/",
                "title": "Rayman Origins: playstation vita: Video Games"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/B006VB2W08/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "",
                "id": "4f4951d26721be000d000004",
                "image_url": "http://ecx.images-amazon.com/images/I/51TcmZUul6L.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f4951d26721be000d000004/",
                "title": "Lumines: Electronic SymphonyGames"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/B005UDTT7C/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "",
                "id": "4f4951e8dd83af000e000002",
                "image_url": "http://ecx.images-amazon.com/images/I/61VPZBc9jtL.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f4951e8dd83af000e000002/",
                "title": "Ultimate Marvel vs Capcom 3: playstation vita"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/B006JKASCK/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "",
                "id": "4f49fe32251fca000e000000",
                "image_url": "http://ecx.images-amazon.com/images/I/51yVozJTUlL.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f49fe32251fca000e000000/",
                "title": "32GB PlayStation Vita Memory Card"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/B002I0GY9G/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "",
                "id": "4f49fe4a80efee000c000000",
                "image_url": "http://ecx.images-amazon.com/images/I/516L0JC1b9L.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f49fe4a80efee000c000000/",
                "title": "Army Corps of Hell"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/B006JKARZS/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "",
                "id": "4f49fe5e58d56d000e000003",
                "image_url": "http://ecx.images-amazon.com/images/I/31lbtT45WjL.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f49fe5e58d56d000e000003/",
                "title": "PlayStation Vita Cradle: Video Games"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/B0050SW93S/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "",
                "id": "4f49fe75251fca000e000002",
                "image_url": "http://ecx.images-amazon.com/images/I/517T81mwtUL.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f49fe75251fca000e000002/",
                "title": "Resistance: Burning Skies"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/B006JI3Q7G/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "",
                "id": "4f49fe9a251fca000c000003",
                "image_url": "http://ecx.images-amazon.com/images/I/51zm67qu-lL.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f49fe9a251fca000c000003/",
                "title": "EA Sports FIFA Soccer"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/B006VB2W0S/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "",
                "id": "4f49feaa80efee000e000000",
                "image_url": "http://ecx.images-amazon.com/images/I/51RWFClN%2B4L.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f49feaa80efee000e000000/",
                "title": "Dungeon Hunter Alliance"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/B006FRNBB2/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "",
                "id": "4f49feba251fca000d000000",
                "image_url": "http://ecx.images-amazon.com/images/I/61VdnLL2SPL.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f49feba251fca000d000000/",
                "title": "Touch My Katamari"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/B006ZPAY46/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "",
                "id": "4f49fec980efee000d000000",
                "image_url": "http://ecx.images-amazon.com/images/I/61igaHsoqyL.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f49fec980efee000d000000/",
                "title": "Unit 13"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/B0074LJ3CE/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "",
                "id": "4f49fed6251fca000d000002",
                "image_url": "http://ecx.images-amazon.com/images/I/51j21mljVPL.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f49fed6251fca000d000002/",
                "title": "Mortal Kombat"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/B006FRNASG/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "",
                "id": "4f49feec80efee000e000002",
                "image_url": "http://ecx.images-amazon.com/images/I/51I7lgmDoTL.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f49feec80efee000e000002/",
                "title": "Shinobido 2: Revenge of Zen"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/B0050SW33E/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "",
                "id": "4f49feff58d56d000e000005",
                "image_url": "http://ecx.images-amazon.com/images/I/51qyuoQCD1L.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f49feff58d56d000e000005/",
                "title": "ModNation Racers"
            }],
            "resource_uri": "/api/v1/my-lists/500/",
            "slug": "vita",
            "title": "Vita"
        },
        {
            "created": "2012-02-25T13:09:29.624082",
            "description": "",
            "id": "499",
            "last_modified_by_user": "2012-02-25T11:59:07.083030",
            "modified": "2012-03-17T21:32:26.631274",
            "owner": {
                "avatar": "/media/avatars/pydanny/resized/80/avatars/pydanny/daniel.greenfeld.jpg",
                "coins": 122,
                "fullname": "Daniel Greenfeld",
                "score": 695,
                "username": "pydanny",
                "waitlisted": false
            },
            "products": [{
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.thinkgeek.com/books/nonfiction/ec9d/%3Fpfm%3Drightcolumn_NewStuffFTW_2",
                "comment": "",
                "id": "4f494e096721be000d000002",
                "image_url": "https://consumernotebook.s3.amazonaws.com/products/www.thinkgeek.com/images/products/frontsquare/ec9d_the_manga_cookbook.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f494e096721be000d000002/",
                "title": "The Manga Cookbook"
            }],
            "resource_uri": "/api/v1/my-lists/499/",
            "slug": "kitchen-fun",
            "title": "Kitchen Fun"
        },
        {
            "created": "2012-02-20T00:58:29.533556",
            "description": "",
            "id": "450",
            "last_modified_by_user": "2012-02-19T17:15:31.026725",
            "modified": "2012-03-17T21:32:27.736434",
            "owner": {
                "avatar": "/media/avatars/pydanny/resized/80/avatars/pydanny/daniel.greenfeld.jpg",
                "coins": 122,
                "fullname": "Daniel Greenfeld",
                "score": 695,
                "username": "pydanny",
                "waitlisted": false
            },
            "products": [{
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.vitaminworld.com/omega-3-and-flaxseed-228/triple-omega-3-6-9-018520",
                "comment": "",
                "id": "4f420b7b758920000b000006",
                "image_url": "http://images.vitaminimages.com/vw/VF/Assets/VitaminWorld_Products/018520.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f420b7b758920000b000006/",
                "title": "Triple Omega 3-6-9 | Coenzyme Q10/CoQ10 Supplements"
            },
            {
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.vitaminworld.com/omega-3-and-flaxseed-228/omega-3-fish-oil-1000-mg-003835",
                "comment": "",
                "id": "4f420b93758920000b000008",
                "image_url": "http://images.vitaminimages.com/vw/VF/Assets/VitaminWorld_Products/003835.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f420b93758920000b000008/",
                "title": "Omega-3 Fish Oil 1000 mg"
            },
            {
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.vitaminworld.com/omega-3-and-flaxseed-228/maximum-strength-triple-omega-3-6-9-010148",
                "comment": "",
                "id": "4f420baae7615d000c00000e",
                "image_url": "http://images.vitaminimages.com/vw/VF/Assets/VitaminWorld_Products/010148.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f420baae7615d000c00000e/",
                "title": "Maximum Strength Triple Omega 3-6-9"
            },
            {
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.vitaminworld.com/omega-3-and-flaxseed-228/wild-salmon-oil-1000-mg-004463",
                "comment": "",
                "id": "4f420be1758920000c000006",
                "image_url": "http://images.vitaminimages.com/vw/VF/Assets/VitaminWorld_Products/004463.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f420be1758920000c000006/",
                "title": "Wild Salmon Oil 1000 mg."
            }],
            "resource_uri": "/api/v1/my-lists/450/",
            "slug": "health-food-and-vitamins",
            "title": "Health Food and vitamins"
        },
        {
            "created": "2012-02-18T22:14:55.262107",
            "description": "",
            "id": "438",
            "last_modified_by_user": "2012-02-18T22:09:23.437132",
            "modified": "2012-03-17T21:32:28.042743",
            "owner": {
                "avatar": "/media/avatars/pydanny/resized/80/avatars/pydanny/daniel.greenfeld.jpg",
                "coins": 122,
                "fullname": "Daniel Greenfeld",
                "score": 695,
                "username": "pydanny",
                "waitlisted": false
            },
            "products": [{
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.performancebike.com/bikes/Product_10052_10551_1094383_-1_1657509_1657508_400327",
                "comment": "",
                "id": "4f40935fefc040000a000000",
                "image_url": "http://media.performancebike.com/images/performance/products/medium/30-4207-BLG-SIDE.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f40935fefc040000a000000/",
                "title": "2011 Fuji Outland 29er 2.0 Mountain Bike"
            },
            {
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.performancebike.com/bikes/Product_10052_10551_1110572_-1_1660010_1660008_400327",
                "comment": "",
                "id": "4f409389759712000c000000",
                "image_url": "http://media.performancebike.com/images/performance/products/medium/30-8976-BLK-SIDE.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f409389759712000c000000/",
                "title": "2012 Diamondback Overdrive 29er Mountain Bike"
            }],
            "resource_uri": "/api/v1/my-lists/438/",
            "slug": "mountain-bikes",
            "title": "Mountain Bikes"
        },
        {
            "created": "2012-02-17T09:33:26.879452",
            "description": "This is where I list all the cycling gear I own or want to own or am evaluating.",
            "id": "428",
            "last_modified_by_user": "2012-02-17T08:20:12.277756",
            "modified": "2012-03-17T21:32:28.275238",
            "owner": {
                "avatar": "/media/avatars/pydanny/resized/80/avatars/pydanny/daniel.greenfeld.jpg",
                "coins": 122,
                "fullname": "Daniel Greenfeld",
                "score": 695,
                "username": "pydanny",
                "waitlisted": false
            },
            "products": [{
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.cleatskins.com/shop/Bikeskins%2520-%2520FullCoverageBikeskins/White",
                "comment": "",
                "id": "4f3e901fe0e026000c000001",
                "image_url": "http://www.cleatskins.com/shop/sites/default/files/imagecache/product/skins-085179%20final%20hero%20copy.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f3e901fe0e026000c000001/",
                "title": "Cleatskins Bikeskins - White | Cleatskins"
            },
            {
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.performancebike.com/bikes/Product_10052_10551_1110572_-1_1660010_1660008_400327",
                "comment": "",
                "id": "4f409389759712000c000000",
                "image_url": "http://media.performancebike.com/images/performance/products/medium/30-8976-BLK-SIDE.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f409389759712000c000000/",
                "title": "2012 Diamondback Overdrive 29er Mountain Bike"
            }],
            "resource_uri": "/api/v1/my-lists/428/",
            "slug": "bicyling",
            "title": "Bicyling"
        },
        {
            "created": "2012-02-16T11:55:24.279846",
            "description": "I need clothes and garments. The workouts are long and glorious, and I'm tired of lugging in an old travel backback.",
            "id": "425",
            "last_modified_by_user": "2012-02-18T13:56:45.549575",
            "modified": "2012-03-17T21:32:28.405261",
            "owner": {
                "avatar": "/media/avatars/pydanny/resized/80/avatars/pydanny/daniel.greenfeld.jpg",
                "coins": 122,
                "fullname": "Daniel Greenfeld",
                "score": 695,
                "username": "pydanny",
                "waitlisted": false
            },
            "products": [{
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.virtualcapoeira.com/info/accessories/pact_show/id_20420782/",
                "comment": "While it would be nice to get something that had Capoeira Batuque on it, this is a nice generic label.",
                "id": "4f3d5f48378789000b000000",
                "image_url": "http://www.virtualcapoeira.com/net/content/9291051201112819505420_300.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f3d5f48378789000b000000/",
                "title": "Capoeira Cinch Pack with Zipper Pocket"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/B00547V62U/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "",
                "id": "4f3d5f88378789000b000001",
                "image_url": "http://ecx.images-amazon.com/images/I/41LP21MqZmL.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f3d5f88378789000b000001/",
                "title": "Hoodie Mens Black \" CAPOEIRA COLOR UP \" Sports: Clothing"
            },
            {
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.virtualcapoeira.com/info/pants/pact_show/id_19386040/%3F",
                "comment": "",
                "id": "4f3d5f9b378789000c000001",
                "image_url": "http://www.virtualcapoeira.com/net/content/92910512006621233358879_300.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f3d5f9b378789000c000001/",
                "title": "Mens White Training Pants | Capoeira Pants for Practicing"
            },
            {
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.virtualcapoeira.com/info/havaianas/pact_show/id_19385982/",
                "comment": "",
                "id": "4f401e2eb5cf53000b000001",
                "image_url": "http://www.virtualcapoeira.com/net/content/92910512006510221942913_300.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f401e2eb5cf53000b000001/",
                "title": "Brazil Havaianas"
            },
            {
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.virtualcapoeira.com/info/atabaques/pact_show/id_19384823/",
                "comment": "",
                "id": "4f401ed75192ba000a000004",
                "image_url": "http://www.virtualcapoeira.com/net/content/92910512008121012593380_500.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f401ed75192ba000a000004/",
                "title": "Atabaque - Improved!"
            },
            {
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.virtualcapoeira.com/info/pandeiros/pact_show/id_19386016/",
                "comment": "",
                "id": "4f401f00b5cf53000b000002",
                "image_url": "http://www.virtualcapoeira.com/net/content/9291051200831193154964_500.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f401f00b5cf53000b000002/",
                "title": "Pandeiro"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/B004QITIAA/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "",
                "id": "4f45afcafac4280100000000",
                "image_url": "http://ecx.images-amazon.com/images/I/51WxYLydVVL.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f45afcafac4280100000000/",
                "title": "Basic Techniques Of Capoeira"
            }],
            "resource_uri": "/api/v1/my-lists/425/",
            "slug": "capoeira-gear",
            "title": "Capoeira Gear"
        },
        {
            "created": "2012-01-19T00:28:26.246811",
            "description": "These are ones with crisp technique, camera, and plot.",
            "id": "420",
            "last_modified_by_user": "2012-02-15T19:39:19.418103",
            "modified": "2012-03-17T21:32:28.513004",
            "owner": {
                "avatar": "/media/avatars/pydanny/resized/80/avatars/pydanny/daniel.greenfeld.jpg",
                "coins": 122,
                "fullname": "Daniel Greenfeld",
                "score": 695,
                "username": "pydanny",
                "waitlisted": false
            },
            "products": [{
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.tkqlhce.com/click-5536662-10475872%3Furl%3Dhttp%253A%252F%252Fwww.bestbuy.com%252Fsite%252Folspage.jsp%253Fid%253D1954262%2526skuId%253D18601525%2526type%253Dproduct%2526ci_src%253D11138%2526ci_sku%253D18601525",
                "comment": "Really good from a technical aspect, this traditional martial arts story is like a step back into some of the post-war films about the Sino-Japanese conflict.",
                "id": "4f3c0176ebae2600040000dd",
                "image_url": "http://images.bestbuy.com/BestBuy_US/images/products/1860/18601525.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f3c0176ebae2600040000dd/",
                "title": "Ip Man - Dubbed Subtitle AC3"
            },
            {
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.jdoqocy.com/click-5536662-10475872%3Furl%3Dhttp%253A%252F%252Fwww.bestbuy.com%252Fsite%252Folspage.jsp%253Fid%253D21522%2526skuId%253D4522369%2526type%253Dproduct%2526ci_src%253D11138%2526ci_sku%253D4522369",
                "comment": "This is the original 1978 film with master kicker Hwang Jang Lee as the bad guy. The subtitled version is infinitely better than the dubbed, because otherwise you will miss the earth, rich Cantonese humor of the period. ",
                "id": "4f3c0187ebae260004000140",
                "image_url": "http://images.bestbuy.com/BestBuy_US/images/products/4522/4522369.jpg",
                "price_range": "$10-20",
                "resource_url": "/api/v1/products/4f3c0187ebae260004000140/",
                "title": "Drunken Master - Widescreen Dubbed Subtitle"
            },
            {
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.tkqlhce.com/click-5536662-10475872%3Furl%3Dhttp%253A%252F%252Fwww.bestbuy.com%252Fsite%252Folspage.jsp%253Fid%253D2181504%2526skuId%253D19008394%2526type%253Dproduct%2526ci_src%253D11138%2526ci_sku%253D19008394",
                "comment": "The sequel to the first Ip Man movie, this is a really good depiction of post-war Hong Kong. The early part of the film has an embellished depiction of the sort of challenges that used to happen in martial arts communities. The later part of the movie is also pretty good, sort of like Rocky I & II but with Kung Fu vs Boxing.",
                "id": "4f3c018bebae26000400016f",
                "image_url": "http://images.bestbuy.com/BestBuy_US/images/products/1900/19008394.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f3c018bebae26000400016f/",
                "title": "Ip Man 2: Legend of the Grandmaster -"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/B005TWGBFW/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "",
                "id": "4f667beaf7793d019f000000",
                "image_url": "http://ecx.images-amazon.com/images/I/51aGV-I3EYL._BO2,204,203,200_PIsitb-sticker-arrow-click,TopRight,35,-76_AA300_SH20_AA278_PIkin4,BottomRight,-67,22_AA300_SH20_OU01_.jpg",
                "price_range": "$50-100",
                "resource_url": "/api/v1/products/4f667beaf7793d019f000000/",
                "title": "How I Proposed to My Wife: An Alien Sex Story eBook: John Scalzi: Kindle Store"
            }],
            "resource_uri": "/api/v1/my-lists/420/",
            "slug": "good-martial-arts-movies",
            "title": "Good Martial Arts movies"
        },
        {
            "created": "2012-01-17T16:17:28.595236",
            "description": "I love Python but I'm doing a lot of Javascript these days. Either in JQuery or MongoDB. These are the books that I live by in my day-to-day efforts as a developer.",
            "id": "418",
            "last_modified_by_user": "2012-02-15T19:39:46.183310",
            "modified": "2012-03-17T21:32:28.551122",
            "owner": {
                "avatar": "/media/avatars/pydanny/resized/80/avatars/pydanny/daniel.greenfeld.jpg",
                "coins": 122,
                "fullname": "Daniel Greenfeld",
                "score": 695,
                "username": "pydanny",
                "waitlisted": false
            },
            "products": [{
                "external_link": "http://www.amazon.com/gp/product/0596517742/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "",
                "id": "4f3c0164ebae260004000040",
                "image_url": "http://ecx.images-amazon.com/images/I/51YIYr01vsL.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f3c0164ebae260004000040/",
                "title": "JavaScript: The Good Parts"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/193398869X/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "",
                "id": "4f3c0192ebae260004000186",
                "image_url": "http://ecx.images-amazon.com/images/I/51jbPsZnqhL.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f3c0192ebae260004000186/",
                "title": "Secrets of the JavaScript Ninja"
            }],
            "resource_uri": "/api/v1/my-lists/418/",
            "slug": "must-have-javascript-books",
            "title": "Must have Javascript books"
        },
        {
            "created": "2012-01-06T20:50:43.350547",
            "description": "Here is a straight-forward list of books I want to read.",
            "id": "396",
            "last_modified_by_user": "2012-02-27T23:25:01.052168",
            "modified": "2012-03-17T21:32:28.681368",
            "owner": {
                "avatar": "/media/avatars/pydanny/resized/80/avatars/pydanny/daniel.greenfeld.jpg",
                "coins": 122,
                "fullname": "Daniel Greenfeld",
                "score": 695,
                "username": "pydanny",
                "waitlisted": false
            },
            "products": [{
                "external_link": "http://www.amazon.com/gp/product/1849515301/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "Numpy book to help me get deep into this amazing library? Yes please!",
                "id": "4f3c0163ebae26000400002d",
                "image_url": "http://ecx.images-amazon.com/images/I/51o0XqA%2BsLL.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f3c0163ebae26000400002d/",
                "title": "NumPy 1.5 Beginner's Guide"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/0596517963/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "I want to learn about licensing and here we go.",
                "id": "4f3c0164ebae260004000054",
                "image_url": "http://ecx.images-amazon.com/images/I/51Wbp2dbB9L.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f3c0164ebae260004000054/",
                "title": "Intellectual Property and Open Source: A Practical Guide to Protecting Code"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/1119998956/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "Design principals that may turn out to be useful",
                "id": "4f3c016aebae26000400009a",
                "image_url": "http://ecx.images-amazon.com/images/I/51SiSPTX2FL.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f3c016aebae26000400009a/",
                "title": "Design for Hackers: Reverse Engineering Beauty"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/0804817162/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "Hard to find but an absolute classic. I kick myself for not buying it in the past when I had the chance.",
                "id": "4f3c016aebae2600040000aa",
                "image_url": "http://ecx.images-amazon.com/images/I/51zESeeKbEL.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f3c016aebae2600040000aa/",
                "title": "The Weapons and Fighting Arts of Indonesia"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/1416555617/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "Steve White and David Weber have an interesting science fiction series and here the former continues to the saga alone. I wish this were on Kindle but here is the paperback for good measure.",
                "id": "4f3c0176ebae2600040000e1",
                "image_url": "http://ecx.images-amazon.com/images/I/515VlhmCUML.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f3c0176ebae2600040000e1/",
                "title": "Exodus (Starfire, Bk. 5)"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/1439134332/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "The follow-up to Exodus by Steve White, this is another paperback Science Fiction book I would love to read.",
                "id": "4f3c0176ebae2600040000e5",
                "image_url": "http://ecx.images-amazon.com/images/I/51mmwkUYj9L.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f3c0176ebae2600040000e5/",
                "title": "Extremis: N/A (Starfire)"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/B0015DROBO/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "Wondering if this is good. It's all over the place so maybe I'll give it a try.",
                "id": "4f3c017cebae26000400012b",
                "image_url": "http://ecx.images-amazon.com/images/I/511x0O8%2B5SL.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f3c017cebae26000400012b/",
                "title": "The Girl with the Dragon Tattoo (Millennium Trilogy)"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/B0043D2E3Q/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "KIndle version of Van Lindburgh's critical work on intellectual property.",
                "id": "4f3c019debae2600040001a8",
                "image_url": "http://ecx.images-amazon.com/images/I/51mP6v3qllL.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f3c019debae2600040001a8/",
                "title": "Intellectual Property and Open Source: A Practical Guide to Protecting Code"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/B002LATV2K/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "By Heresies Distressed picks up exactly at the end of Book 2 of the safehold series. As the reformation gets into swing, the world leaps into turmoil.",
                "id": "4f3c019eebae2600040001bb",
                "image_url": "http://ecx.images-amazon.com/images/I/51PKqNsiHPL.jpg",
                "price_range": "$0-10",
                "resource_url": "/api/v1/products/4f3c019eebae2600040001bb/",
                "title": "By Heresies Distressed"
            },
            {
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.packtpub.com/numpy-1-5-using-real-world-examples-beginners-guide/book%23author",
                "comment": "",
                "id": "4f44f78e358859000b00000b",
                "image_url": "https://www.packtpub.com/sites/default/files/imagecache/productview_ebook/5306OS_NumPy%201.5_FrontCover.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f44f78e358859000b00000b/",
                "title": "NumPy 1.5 Beginner's Guide | Packt Publishing Technical & IT Book and eBook Store"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/3540739157/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "",
                "id": "4f44f8565602c3000a000003",
                "image_url": "http://ecx.images-amazon.com/images/I/41N6MyO%2BIIL.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f44f8565602c3000a000003/",
                "title": "Python Scripting for Computational Science  Hans Petter Langtangen"
            },
            {
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.packtpub.com/matplotlib-python-development/book",
                "comment": "",
                "id": "4f44f92f3b0a04000c000004",
                "image_url": "https://www.packtpub.com/sites/default/files/imagecache/productview_ebook/bookimages/4947_MockupCover.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f44f92f3b0a04000c000004/",
                "title": "Matplotlib for Python Developers | Packt Publishing Technical & IT Book and eBook Store"
            },
            {
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.tramy.us/",
                "comment": "",
                "id": "4f44f9d65602c3000c000009",
                "image_url": "http://www.tramy.us/setfree_small.png",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f44f9d65602c3000c000009/",
                "title": "Guide to Numpy Travis E. Oliphant"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/1430218436/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "",
                "id": "4f4501af3b0a04000a000008",
                "image_url": "http://ecx.images-amazon.com/images/I/51ww9Itv0RL.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f4501af3b0a04000a000008/",
                "title": "Beginning Python Visualization: Crafting Visual Transformation"
            },
            {
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.thinkgeek.com/books/nonfiction/ec9d/%3Fpfm%3Drightcolumn_NewStuffFTW_2",
                "comment": "",
                "id": "4f494e096721be000d000002",
                "image_url": "https://consumernotebook.s3.amazonaws.com/products/www.thinkgeek.com/images/products/frontsquare/ec9d_the_manga_cookbook.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f494e096721be000d000002/",
                "title": "The Manga Cookbook"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/0316007625/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "",
                "id": "4f49b7c3feac66000d000000",
                "image_url": "http://ecx.images-amazon.com/images/I/51ycgh845CL.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f49b7c3feac66000d000000/",
                "title": "Shark vs. Train by Chris Barton, Tom Lichtenheld"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/0399526145/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "",
                "id": "4f5054f57eb9f6000c000000",
                "image_url": "http://ecx.images-amazon.com/images/I/51xd5JLUbDL.jpg",
                "price_range": "$20-50",
                "resource_url": "/api/v1/products/4f5054f57eb9f6000c000000/",
                "title": "The 7 Powers of Questions: Secrets to Successful Communication in Life and at Work by Dorothy Leeds"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/1573920355/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "Copernicus changed the world with this book.",
                "id": "4f53dc64fe40db000e000000",
                "image_url": "http://ecx.images-amazon.com/images/I/41UVdLKeROL.jpg",
                "price_range": "$10-20",
                "resource_url": "/api/v1/products/4f53dc64fe40db000e000000/",
                "title": "On the Revolutions of Heavenly Spheres by Nicolaus Copernicus: Books"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/4770028016/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "I've read this book a few times, but I just want this nice collector's version.",
                "id": "4f5811d5a2fb42000e000000",
                "image_url": "http://ecx.images-amazon.com/images/I/51FIg2hszaL.jpg",
                "price_range": "$50-100",
                "resource_url": "/api/v1/products/4f5811d5a2fb42000e000000/",
                "title": "The Book of Five Rings (Bushido--The Way of the Warrior) (9784770028013): Miyamoto Musashi, William "
            },
            {
                "external_link": "http://www.amazon.com/gp/product/B005OTDQQ2/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "I really like Scalzi's \"Old Man\" universe. This is stories from the point of view of Jane Sagan.",
                "id": "4f650c89931314000d000000",
                "image_url": "http://ecx.images-amazon.com/images/I/51vvGdFBs1L.jpg",
                "price_range": "$0-10",
                "resource_url": "/api/v1/products/4f650c89931314000d000000/",
                "title": "The Sagan Diary eBook: John Scalzi: Kindle Store"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/B005OTEEEA/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "",
                "id": "4f657b759007d7000e000002",
                "image_url": "http://ecx.images-amazon.com/images/I/51CuKsKGF8L.jpg",
                "price_range": "$0-10",
                "resource_url": "/api/v1/products/4f657b759007d7000e000002/",
                "title": "Questions for a Soldier eBook: John Scalzi"
            }],
            "resource_uri": "/api/v1/my-lists/396/",
            "slug": "book-wishlist",
            "title": "Book wishlist"
        },
        {
            "created": "2012-01-04T10:11:03.055199",
            "description": "These are pieces I want to have in my house.",
            "id": "381",
            "last_modified_by_user": "2012-01-04T17:00:06.062991",
            "modified": "2012-03-17T21:32:28.993570",
            "owner": {
                "avatar": "/media/avatars/pydanny/resized/80/avatars/pydanny/daniel.greenfeld.jpg",
                "coins": 122,
                "fullname": "Daniel Greenfeld",
                "score": 695,
                "username": "pydanny",
                "waitlisted": false
            },
            "products": [{
                "external_link": "http://www.amazon.com/gp/product/B001AQ6GJW/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "An Elephant table would go well with the Zebra Accent chair.",
                "id": "4f3c017debae26000400013b",
                "image_url": "http://ecx.images-amazon.com/images/I/41ZD%2BE7s9OL.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f3c017debae26000400013b/",
                "title": "Two's Company Elephant Side Table Ceramic"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/B005XEHTKM/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "This chair would look great in a room with an indoor pool full of lovely dappled sunlight coming through the windows.",
                "id": "4f3c01a9ebae260004000245",
                "image_url": "http://ecx.images-amazon.com/images/I/41xhGQ2NoQL.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f3c01a9ebae260004000245/",
                "title": "Deco Zebra Accent Chair"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/B00166DR9S/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "need a new chair",
                "id": "4f5a7c07204d33000c000001",
                "image_url": "http://ecx.images-amazon.com/images/I/4158fFJJcUL.jpg",
                "price_range": "$100-200",
                "resource_url": "/api/v1/products/4f5a7c07204d33000c000001/",
                "title": "Boss Black LeatherPlus Executive Chair"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/B002ZDUDV6/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "Yet another chair.",
                "id": "4f5a85d8310cb0000c000002",
                "image_url": "http://ecx.images-amazon.com/images/I/312qZgDBpML.jpg",
                "price_range": "$100-200",
                "resource_url": "/api/v1/products/4f5a85d8310cb0000c000002/",
                "title": "Flash furniture Black Leather Office Chair, GO-7194B-BK-GG: Office Products"
            }],
            "resource_uri": "/api/v1/my-lists/381/",
            "slug": "furniture-wishlist",
            "title": "Furniture Wishlist"
        },
        {
            "created": "2012-01-03T09:07:19.577826",
            "description": "I love documentaries!",
            "id": "378",
            "last_modified_by_user": "2012-01-03T23:35:38.095761",
            "modified": "2012-03-17T21:32:29.063358",
            "owner": {
                "avatar": "/media/avatars/pydanny/resized/80/avatars/pydanny/daniel.greenfeld.jpg",
                "coins": 122,
                "fullname": "Daniel Greenfeld",
                "score": 695,
                "username": "pydanny",
                "waitlisted": false
            },
            "products": [{
                "external_link": "http://www.amazon.com/gp/product/B000FGG5GC/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "The story of how Capoeira came to Switzerland. Not sure if it is any good but it seems interesting.",
                "id": "4f3c018bebae26000400016a",
                "image_url": "http://ecx.images-amazon.com/images/I/51CdGyy0zsL.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f3c018bebae26000400016a/",
                "title": "Capoeira"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/B000GTJSFS/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "My favorite Dinosaur documentary",
                "id": "4f3c019febae2600040001d2",
                "image_url": "http://ecx.images-amazon.com/images/I/515caNGeHyL.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f3c019febae2600040001d2/",
                "title": "Walking with Dinosaurs"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/B000MRAAJM/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "David A talking about planet Earth!",
                "id": "4f3c01a9ebae26000400023b",
                "image_url": "http://ecx.images-amazon.com/images/I/51vOcFKASRL.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f3c01a9ebae26000400023b/",
                "title": "Planet Earth: The Complete BBC Series [Blu-ray]"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/B004HFKPOK/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "More terrifying than any horror movie because this is the real world.",
                "id": "4f3c01afebae26000400027d",
                "image_url": "http://ecx.images-amazon.com/images/I/515HnSnQbeL.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f3c01afebae26000400027d/",
                "title": "Inside North Korea"
            }],
            "resource_uri": "/api/v1/my-lists/378/",
            "slug": "documentaries",
            "title": "Documentaries"
        },
        {
            "created": "2011-12-29T22:50:57.348589",
            "description": "We built Consumer Notebook with Django as one of the components. Here are a set of references that are available for study.",
            "id": "363",
            "last_modified_by_user": "2011-12-29T23:04:00.254225",
            "modified": "2012-03-17T21:32:29.358600",
            "owner": {
                "avatar": "/media/avatars/pydanny/resized/80/avatars/pydanny/daniel.greenfeld.jpg",
                "coins": 122,
                "fullname": "Daniel Greenfeld",
                "score": 695,
                "username": "pydanny",
                "waitlisted": false
            },
            "products": [{
                "external_link": "http://www.amazon.com/gp/product/1430210478/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "Marty Alchin's book is AMAZING. This won't just make your Django skills better, it will make your Python and programming skills jump in prowess. If you get any book in this list, get this one!!!",
                "id": "4f3c0164ebae260004000043",
                "image_url": "http://ecx.images-amazon.com/images/I/41Ry%2BLUNkQL.jpg",
                "price_range": "$20-50",
                "resource_url": "/api/v1/products/4f3c0164ebae260004000043/",
                "title": "Pro Django (Expert's Voice in Web Development)"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/143021936X/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "A bit dated, but still quite handy. I honed much of my Django skills on an earlier version of this book.",
                "id": "4f3c0168ebae260004000070",
                "image_url": "http://ecx.images-amazon.com/images/I/5198kKFjb2L.jpg",
                "price_range": "$20-50",
                "resource_url": "/api/v1/products/4f3c0168ebae260004000070/",
                "title": "The Definitive Guide to Django: Web Development Done Right"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/1847197000/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "This books is terrible. The code is broken. Don't buy it!",
                "id": "4f3c0177ebae260004000100",
                "image_url": "http://ecx.images-amazon.com/images/I/41xUMvA8nUL.jpg",
                "price_range": "$20-50",
                "resource_url": "/api/v1/products/4f3c0177ebae260004000100/",
                "title": "Django 1.2 e-commerce"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/0132356139/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "Wesley Chun is a hero of mine, and Jeff Forcier is the guy behind Fabric. Together along with Paul Bissex they deliver a serious book for experienced Python and Django developers. However, I think this book will be hard for incoming developers.",
                "id": "4f3c0188ebae26000400014e",
                "image_url": "http://ecx.images-amazon.com/images/I/41c1QK1THKL.jpg",
                "price_range": "$20-50",
                "resource_url": "/api/v1/products/4f3c0188ebae26000400014e/",
                "title": "Python Web Development with Django"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/B006OYO9SK/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "I have some concerns that this is using the old local_settings.py method of controlling domain specific settings. Nevertheless, it's good to see more people stepping into the role of documenters.",
                "id": "4f3c018aebae26000400015c",
                "image_url": "http://ecx.images-amazon.com/images/I/312kliN4qdL.jpg",
                "price_range": "$20-50",
                "resource_url": "/api/v1/products/4f3c018aebae26000400015c/",
                "title": "Django Design Patterns"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/1847197566/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "Karen Tracey is a Django core developer and is a powerful authority on testing. This book is another handy reference for any serious Django developer.",
                "id": "4f3c019febae2600040001d0",
                "image_url": "http://ecx.images-amazon.com/images/I/41A0xBtW5PL.jpg",
                "price_range": "$20-50",
                "resource_url": "/api/v1/products/4f3c019febae2600040001d0/",
                "title": "Django 1.1 Testing and Debugging"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/1847196780/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "Really good book for getting bootstrapped into Django. ",
                "id": "4f3c01aaebae260004000258",
                "image_url": "http://ecx.images-amazon.com/images/I/511QYiLPJbL.jpg",
                "price_range": "$20-50",
                "resource_url": "/api/v1/products/4f3c01aaebae260004000258/",
                "title": "Django 1.0 Website Development"
            }],
            "resource_uri": "/api/v1/my-lists/363/",
            "slug": "django-books",
            "title": "Django Books"
        },
        {
            "created": "2011-12-28T23:26:51.995378",
            "description": "How can anyone go wrong with Lego based video games?",
            "id": "354",
            "last_modified_by_user": "2011-12-28T23:29:55.634628",
            "modified": "2012-03-17T21:32:29.567544",
            "owner": {
                "avatar": "/media/avatars/pydanny/resized/80/avatars/pydanny/daniel.greenfeld.jpg",
                "coins": 122,
                "fullname": "Daniel Greenfeld",
                "score": 695,
                "username": "pydanny",
                "waitlisted": false
            },
            "products": [{
                "external_link": "http://www.amazon.com/gp/product/B0010YOQJQ/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "Cue dramatic pulp action and pulse-pouding music when you play as Indiana Jones in a world of Legos.",
                "id": "4f3c0177ebae2600040000f5",
                "image_url": "http://ecx.images-amazon.com/images/I/51QEGrxvkcL.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f3c0177ebae2600040000f5/",
                "title": "Lego Indiana Jones: The Original Adventures"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/B000ZKBJY6/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "Fight injustice as the Batman in a Lego version of Gotham city!",
                "id": "4f3c019febae2600040001ce",
                "image_url": "http://ecx.images-amazon.com/images/I/517zan%2Bv3eL.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f3c019febae2600040001ce/",
                "title": "Lego Batman"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/B000G7X0AO/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "Play through the original Star Wars series as Lego characters!",
                "id": "4f3c019febae2600040001e0",
                "image_url": "http://ecx.images-amazon.com/images/I/51I5gVRtCWL.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f3c019febae2600040001e0/",
                "title": "Lego Star Wars II: The Original Trilogy"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/B0037UCTCW/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "Battle the nefarious robot armies as brave jedi!",
                "id": "4f3c01adebae260004000266",
                "image_url": "http://ecx.images-amazon.com/images/I/514B%2Bw86lIL.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f3c01adebae260004000266/",
                "title": "LEGO Star Wars III The Clone Wars"
            }],
            "resource_uri": "/api/v1/my-lists/354/",
            "slug": "lego-video-games",
            "title": "Lego Video Games"
        },
        {
            "created": "2011-12-27T18:18:06.972592",
            "description": "This is a list about Zombies. Books, games, movies, and more!",
            "id": "342",
            "last_modified_by_user": "2012-02-15T23:44:57.683994",
            "modified": "2012-03-17T21:32:29.663230",
            "owner": {
                "avatar": "/media/avatars/pydanny/resized/80/avatars/pydanny/daniel.greenfeld.jpg",
                "coins": 122,
                "fullname": "Daniel Greenfeld",
                "score": 695,
                "username": "pydanny",
                "waitlisted": false
            },
            "products": [{
                "external_link": "http://www.amazon.com/gp/product/1400049628/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "I received this as a birthday present in July of 2011 from Grant and Sophia Viklund.",
                "id": "4f3c016aebae2600040000b4",
                "image_url": "http://ecx.images-amazon.com/images/I/51kfZ29lrGL.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f3c016aebae2600040000b4/",
                "title": "The Zombie Survival Guide: Complete Protection from the Living Dead"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/B003IKMR0U/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "This is supposed to a fun, silly game that is easy to learn and play.",
                "id": "4f3c017aebae260004000116",
                "image_url": "http://ecx.images-amazon.com/images/I/51S48Jj28IL.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f3c017aebae260004000116/",
                "title": "Zombie Dice"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/1569763429/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "In case you get turned into a Zombie, this is a guide as to what you should be doing!",
                "id": "4f3c0188ebae260004000142",
                "image_url": "http://ecx.images-amazon.com/images/I/51gQHCAlRaL.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f3c0188ebae260004000142/",
                "title": "So Now You're a Zombie: A Handbook for the Newly Undead (Humour)"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/B000JMKQX0/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "I love how Max Brooks channels Studs Turkel in writing about the great Zombie war and how mankind was chased into near extinction and yet manages to survive against the odds.",
                "id": "4f3c019eebae2600040001cc",
                "image_url": "http://ecx.images-amazon.com/images/I/51d2Jv0LZTL.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f3c019eebae2600040001cc/",
                "title": "World War Z: An Oral History of the Zombie War"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/B0018OIK0E/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "",
                "id": "4f3cb43a5e73c2000c000000",
                "image_url": "http://ecx.images-amazon.com/images/I/51bRrMdvLtL.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f3cb43a5e73c2000c000000/",
                "title": "Shaun of the Dead"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/B0030B624E/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "",
                "id": "4f3cb47a5e73c2000b000000",
                "image_url": "http://ecx.images-amazon.com/images/I/51NgH8TbMtL.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f3cb47a5e73c2000b000000/",
                "title": "Zombieland: Amazon Instant Video"
            }],
            "resource_uri": "/api/v1/my-lists/342/",
            "slug": "zombies",
            "title": "Zombies"
        },
        {
            "created": "2011-12-26T11:25:19.509885",
            "description": "These are board games where instead of competing together you tend to work together to win a common goal.",
            "id": "337",
            "last_modified_by_user": "2011-12-28T15:21:44.191176",
            "modified": "2012-03-17T21:32:29.724028",
            "owner": {
                "avatar": "/media/avatars/pydanny/resized/80/avatars/pydanny/daniel.greenfeld.jpg",
                "coins": 122,
                "fullname": "Daniel Greenfeld",
                "score": 695,
                "username": "pydanny",
                "waitlisted": false
            },
            "products": [{
                "external_link": "http://www.amazon.com/gp/product/B003D7F4YY/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "You and the other players are racing to rescue archeological treasures from a sinking island. Work together to save these pieces or sink to a watery doom!",
                "id": "4f3c0161ebae26000400000d",
                "image_url": "http://ecx.images-amazon.com/images/I/51UmKMROcNL.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f3c0161ebae26000400000d/",
                "title": "Forbidden Island"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/1589944607/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "Work together to save the remainder of humanity from the Cylons. Unfortunately one player is a Cylon agent and rooting that person out is the only way to save humanity.",
                "id": "4f3c0164ebae260004000053",
                "image_url": "http://ecx.images-amazon.com/images/I/41MEFeBm9XL.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f3c0164ebae260004000053/",
                "title": "Battlestar Galactica"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/B0013OBXG2/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "Cooperate with the other players to find the cures to 4 terrible plagues or humanity perishes into the night.",
                "id": "4f3c016aebae2600040000ad",
                "image_url": "http://ecx.images-amazon.com/images/I/51Zt7Dh94zL.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f3c016aebae2600040000ad/",
                "title": "Pandemic"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/1616611693/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "Gears of War is a very popular video game franchise, and in this board game you and the other players make up a squad trying to accomplish missions against the locusts.",
                "id": "4f3c0188ebae26000400014b",
                "image_url": "http://ecx.images-amazon.com/images/I/51TPRDWORcL.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f3c0188ebae26000400014b/",
                "title": "Gears Of War The Board Game"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/0975277383/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "Imagine playing as knights of King Arthur's Court; which means righting wrongs and correcting injustices, all while trying to keep the fall of the kingdom at bay. In larger games one player becomes the betrayer and tension is added to the play as rooting out this person becomes more and more important. Tons of fun!",
                "id": "4f3c019eebae2600040001c7",
                "image_url": "http://ecx.images-amazon.com/images/I/61X8ILdd7qL.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f3c019eebae2600040001c7/",
                "title": "Shadows Over Camelot"
            }],
            "resource_uri": "/api/v1/my-lists/337/",
            "slug": "cooperative-board-games",
            "title": "Cooperative Board Games"
        },
        {
            "created": "2011-12-23T14:02:36.077775",
            "description": "These are all one-use items that may not be practical all the time, but they are fun to have around for special occasions.",
            "id": "324",
            "last_modified_by_user": "2012-01-05T11:14:54.613236",
            "modified": "2012-03-17T21:32:29.791540",
            "owner": {
                "avatar": "/media/avatars/pydanny/resized/80/avatars/pydanny/daniel.greenfeld.jpg",
                "coins": 122,
                "fullname": "Daniel Greenfeld",
                "score": 695,
                "username": "pydanny",
                "waitlisted": false
            },
            "products": [{
                "external_link": "http://www.amazon.com/gp/product/B00018RR48/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "Fondue is fun and yummy.",
                "id": "4f3c0163ebae260004000027",
                "image_url": "http://ecx.images-amazon.com/images/I/41HAPjD%2BZXL.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f3c0163ebae260004000027/",
                "title": "Cuisinart CFO-3SS Electric Fondue Maker"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/B000FFVJ3C/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "I love dehydrated fruit. This seems like such a wonderful thing. Can you dehydrate a person with not much of a brain?",
                "id": "4f3c0164ebae26000400003b",
                "image_url": "http://ecx.images-amazon.com/images/I/41KNN0N17BL.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f3c0164ebae26000400003b/",
                "title": "Nesco FD-75PR 700-Watt Food Dehydrator"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/B001E5CWVU/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "Good for not filling up your oven with something that takes hours to cook. Also allows you to carry your kitchen efforts to other locations.",
                "id": "4f3c0169ebae260004000086",
                "image_url": "http://ecx.images-amazon.com/images/I/41OtZjbJHsL.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f3c0169ebae260004000086/",
                "title": "Cuisinart PSC-350 3-1/2-Quart Programmable Slow Cooker"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/B002JM100Q/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "Giant corn popper thingee!",
                "id": "4f3c016aebae260004000099",
                "image_url": "http://ecx.images-amazon.com/images/I/41ZqYL-RUCL.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f3c016aebae260004000099/",
                "title": "West Bend 82386 Kettle Krazy Popcorn Popper and Nut Roaster"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/B001P2J3K0/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "This seems like an awesome fruit dryer. Shelves! I think this is the one I want.",
                "id": "4f3c016aebae2600040000a3",
                "image_url": "http://ecx.images-amazon.com/images/I/41S5bKbppZL.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f3c016aebae2600040000a3/",
                "title": "Excalibur 3900 Deluxe Series 9 Tray Food Dehydrator - Black"
            },
            {
                "external_link": "http://www.amazon.com/gp/product/B005D6FWCC/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "comment": "Great for any event! Large so the lazy susan property of this device is a a necessity.",
                "id": "4f3c01afebae260004000282",
                "image_url": "http://ecx.images-amazon.com/images/I/41w8FbzTGuL.jpg",
                "price_range": "Coming",
                "resource_url": "/api/v1/products/4f3c01afebae260004000282/",
                "title": "Crock-Pot SCRTD305-BS 1-Quart Triple Dipper Food Warmer, Stainless Steel"
            }],
            "resource_uri": "/api/v1/my-lists/324/",
            "slug": "fun-home-appliances",
            "title": "Fun Home Appliances"
        }]
    }