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
                "link": "https://consumernotebook.com/motionsports-adrenaline-xbox/4f59a086204d33000e000000/",
                "price_range": "$50-100",
                "resource_uri": "/api/v1/products/4f59a086204d33000e000000/",
                "title": "MotionSports Adrenaline: XBox"
            },
            {
                "comment": "A super heroku fight game? Sign me up!",
                "external_link": "http://www.amazon.com/gp/product/B004U9T6FM/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f59a0f55ddae9000d000000",
                "image_url": "http://ecx.images-amazon.com/images/I/61j1tcm6ZjL.jpg",
                "link": "https://consumernotebook.com/powerup-heroes-xbox/4f59a0f55ddae9000d000000/",
                "price_range": "$20-50",
                "resource_uri": "/api/v1/products/4f59a0f55ddae9000d000000/",
                "title": "PowerUP Heroes: XBox"
            },
            {
                "comment": "I like games",
                "external_link": "http://www.amazon.com/gp/product/B002I0H8FK/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f5b9c9f24b4b3000e000003",
                "image_url": "http://ecx.images-amazon.com/images/I/5109BtpAZPL.jpg",
                "link": "https://consumernotebook.com/child-of-eden-xbox-360-video-games/4f5b9c9f24b4b3000e000003/",
                "price_range": "$20-50",
                "resource_uri": "/api/v1/products/4f5b9c9f24b4b3000e000003/",
                "title": "Child Of Eden: Xbox 360: Video Games"
            },
            {
                "comment": "deepak!",
                "external_link": "http://www.amazon.com/gp/product/B0056WJA3K/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f5b9e1736a633000d000006",
                "image_url": "http://ecx.images-amazon.com/images/I/51llqktiEZL.jpg",
                "link": "https://consumernotebook.com/deepak-chopras-leela-xbox-360-video-games/4f5b9e1736a633000d000006/",
                "price_range": "$20-50",
                "resource_uri": "/api/v1/products/4f5b9e1736a633000d000006/",
                "title": "Deepak Chopra's Leela: Xbox 360: Video Games"
            },
            {
                "comment": "Dance!",
                "external_link": "http://www.amazon.com/gp/product/B00061NL7W/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f5ba47936a633000e000006",
                "image_url": "http://ecx.images-amazon.com/images/I/51vm-es1RUL.jpg",
                "link": "https://consumernotebook.com/yourself-fitness-xbox/4f5ba47936a633000e000006/",
                "price_range": "$50-100",
                "resource_uri": "/api/v1/products/4f5ba47936a633000e000006/",
                "title": "Yourself Fitness: Xbox:"
            },
            {
                "comment": "guy is punching!",
                "external_link": "http://www.amazon.com/gp/product/B002I0H9WM/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f5bab081cfd5d000c000008",
                "image_url": "http://ecx.images-amazon.com/images/I/51gcyDU9V%2BL.jpg",
                "link": "https://consumernotebook.com/your-shape-fitness-evolved-video-games/4f5bab081cfd5d000c000008/",
                "price_range": "$50-100",
                "resource_uri": "/api/v1/products/4f5bab081cfd5d000c000008/",
                "title": "Your Shape Fitness Evolved: Video Games"
            }],
            "resource_uri": "/api/v1/lists/pydanny/kinect-games/",
            "slug": "kinect-games",
            "title": "Kinect Games",
            "url": "http://consumernotebook.com/lists/pydanny/kinect-games/"
        },
        {
            "created": "2012-03-06T17:18:52.312598",
            "description": "",
            "id": "530",
            "last_modified_by_user": "2012-03-06T17:07:08.617723",
            "modified": "2012-03-18T21:33:29.700795",
            "owner": {
                "avatar": "/media/avatars/pydanny/resized/80/avatars/pydanny/daniel.greenfeld.jpg",
                "coins": 122,
                "fullname": "Daniel Greenfelds",
                "score": 695,
                "username": "pydanny",
                "waitlisted": false
            },
            "products": [{
                "comment": "Discover is a good mix of articles over a wide range of subjects. Also, it's website is served out with the Python programming language.",
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.magazinediscountcenter.com/magazine-subscription/Discover.html",
                "id": "4f56b77cda8e7c000c000000",
                "image_url": "http://www.magazinediscountcenter.com/images/prod_images/large/363.jpg",
                "link": "https://consumernotebook.com/discover-magazine/4f56b77cda8e7c000c000000/",
                "price_range": "$20-50",
                "resource_uri": "/api/v1/products/4f56b77cda8e7c000c000000/",
                "title": "Discover Magazine"
            },
            {
                "comment": "Sue me, I love the pretty space pictures in this magazine. No matter how good monitors get, you can't get the same thing electronically.",
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.magazinediscountcenter.com/magazine-subscription/Science-Illustrated.html",
                "id": "4f56b7ccdd779f000d000000",
                "image_url": "http://www.magazinediscountcenter.com/images/prod_images/large/800.jpg",
                "link": "https://consumernotebook.com/science-illustrated-magazine/4f56b7ccdd779f000d000000/",
                "price_range": "$20-50",
                "resource_uri": "/api/v1/products/4f56b7ccdd779f000d000000/",
                "title": "Science Illustrated Magazine"
            },
            {
                "comment": "I started reading this recently thanks to my electrician. While waiting ro the inspector, he had a few in his van. ",
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.magazinediscountcenter.com/magazine-subscription/Scientific-American.html",
                "id": "4f56b857dd779f000d000002",
                "image_url": "http://www.magazinediscountcenter.com/images/prod_images/large/714.jpg",
                "link": "https://consumernotebook.com/scientific-american-magazine/4f56b857dd779f000d000002/",
                "price_range": "$20-50",
                "resource_uri": "/api/v1/products/4f56b857dd779f000d000002/",
                "title": "Scientific American Magazine"
            }],
            "resource_uri": "/api/v1/lists/pydanny/magazines-i-should-read/",
            "slug": "magazines-i-should-read",
            "title": "Magazines I should read",
            "url": "http://consumernotebook.com/lists/pydanny/magazines-i-should-read/"
        },
        {
            "created": "2012-03-04T21:47:02.773453",
            "description": "It can be hard to buy gifts for an active, retired mom. These are nice, affordable gifts any mother would love.",
            "id": "523",
            "last_modified_by_user": "2012-03-04T22:15:18.861270",
            "modified": "2012-03-18T21:33:30.135866",
            "owner": {
                "avatar": "/media/avatars/pydanny/resized/80/avatars/pydanny/daniel.greenfeld.jpg",
                "coins": 122,
                "fullname": "Daniel Greenfelds",
                "score": 695,
                "username": "pydanny",
                "waitlisted": false
            },
            "products": [{
                "comment": "My mom stays really healthy through good eating of lighter foods. This is an awesome periodical to help her out.",
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.magazinediscountcenter.com/magazine-subscription/Cooking-Light.html",
                "id": "4f5439c1ba376c000c000000",
                "image_url": "https://consumernotebook.s3.amazonaws.com/products/www.magazinediscountcenter.com/images/prod_images/large/331.jpg",
                "link": "https://consumernotebook.com/cooking-light-magazine/4f5439c1ba376c000c000000/",
                "price_range": "$20-50",
                "resource_uri": "/api/v1/products/4f5439c1ba376c000c000000/",
                "title": "Cooking Light Magazine"
            },
            {
                "comment": "This is great for any garden, large or small. Mom can pack in a lot of herbs or flowers into a small location in a very attractive package.",
                "external_link": "http://www.amazon.com/gp/product/B002IYHIKG/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f5453dfb15ef7000e000000",
                "image_url": "http://ecx.images-amazon.com/images/I/41%2Bz99pmfVL.jpg",
                "link": "https://consumernotebook.com/akro-mils-stack-a-pot/4f5453dfb15ef7000e000000/",
                "price_range": "$20-50",
                "resource_uri": "/api/v1/products/4f5453dfb15ef7000e000000/",
                "title": "Akro-Mils Stack-A-Pot"
            },
            {
                "comment": "Yoga has been taken up by a lot of active, retired moms. This mat stays odor free pretty much forever, and is thick enough to keep joints off cold, hard floors.",
                "external_link": "http://www.amazon.com/gp/product/B004TN51EE/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f54546cb15ef7000e000002",
                "image_url": "http://ecx.images-amazon.com/images/I/41i3G25PRZL.jpg",
                "link": "https://consumernotebook.com/aurorae-classic-yoga-mat-always-smells-good/4f54546cb15ef7000e000002/",
                "price_range": "$20-50",
                "resource_uri": "/api/v1/products/4f54546cb15ef7000e000002/",
                "title": "Aurorae Classic Yoga Mat - Always smells good."
            },
            {
                "comment": "Because of their longevity, moms often prefer plants over flowers. ",
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.flowersacrossamerica.com/product.cfm%3Fdcode%3DC26-2943",
                "id": "4f5459dfb15ef7000c000006",
                "image_url": "http://www.flowersacrossamerica.com/flowers/products/C26-2943.jpg",
                "link": "https://consumernotebook.com/french-garden-best-selling-flowers/4f5459dfb15ef7000c000006/",
                "price_range": "$50-100",
                "resource_uri": "/api/v1/products/4f5459dfb15ef7000c000006/",
                "title": "French Garden - Best Selling Flowers"
            },
            {
                "comment": "On the pricey side of things, this ultrabook has the grace of the MacBook Air and the familiarity of Windows.",
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.newegg.com/Product/Product.aspx%3FItem%3DN82E16834230171",
                "id": "4f545c01b15ef7000c000008",
                "image_url": "http://images17.newegg.com/is/image/newegg/34-230-171-TS?$S300W$",
                "link": "https://consumernotebook.com/asus-zenbook-ux31e-dh52-ultrabook-i5-170ghz-133-4gb-128gb-ssd-hdd/4f545c01b15ef7000c000008/",
                "price_range": "$1000-2000",
                "resource_uri": "/api/v1/products/4f545c01b15ef7000c000008/",
                "title": "ASUS Zenbook UX31E-DH52 Ultrabook i5 1.70GHz 13.3\" 4GB  128GB SSD HDD"
            },
            {
                "comment": "A nicely affordable laptop to give your mom, the Asus brand is known for their quality components and assembly.",
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.newegg.com/Product/Product.aspx%3FItem%3DN82E16834230359",
                "id": "4f545ceeb15ef7000e000004",
                "image_url": "http://images10.newegg.com/NeweggImage/ProductImageCompressAll300/34-230-359-02.jpg",
                "link": "https://consumernotebook.com/asus-eee-pc-matte-black-intel-atom-n2600-160ghz-101-1gb-ddr3-memory-320gb-hdd-netbook/4f545ceeb15ef7000e000004/",
                "price_range": "$200-500",
                "resource_uri": "/api/v1/products/4f545ceeb15ef7000e000004/",
                "title": "ASUS Eee PC Matte Black Intel Atom N2600, 1.60GHz 10.1\" 1GB DDR3 Memory 320GB HDD Netbook"
            },
            {
                "comment": "She types a lot.",
                "external_link": "http://www.amazon.com/gp/product/B00166DR9S/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f5a7c07204d33000c000001",
                "image_url": "http://ecx.images-amazon.com/images/I/4158fFJJcUL.jpg",
                "link": "https://consumernotebook.com/boss-black-leatherplus-executive-chair/4f5a7c07204d33000c000001/",
                "price_range": "$100-200",
                "resource_uri": "/api/v1/products/4f5a7c07204d33000c000001/",
                "title": "Boss Black LeatherPlus Executive Chair"
            }],
            "resource_uri": "/api/v1/lists/pydanny/gifts-to-give-your-retired-mom/",
            "slug": "gifts-to-give-your-retired-mom",
            "title": "Gifts to give your retired mom",
            "url": "http://consumernotebook.com/lists/pydanny/gifts-to-give-your-retired-mom/"
        },
        {
            "created": "2012-02-26T16:57:07.354140",
            "description": "Help me fill this out. Send me recommendations to my twitter account as pydanny.",
            "id": "503",
            "last_modified_by_user": "2012-02-27T09:41:07.737663",
            "modified": "2012-03-18T21:33:31.089989",
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
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//macromates.com/",
                "id": "4f4ad4e35a4305000d000000",
                "image_url": "https://consumernotebook.s3.amazonaws.com/products/manual.macromates.com/images/project_window_with_tabs.png",
                "link": "https://consumernotebook.com/textmate-the-missing-editor-for-mac-os-x/4f4ad4e35a4305000d000000/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f4ad4e35a4305000d000000/",
                "title": "TextMate: The Missing Editor for Mac OS X"
            },
            {
                "comment": "",
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.sublimetext.com/",
                "id": "4f4ad53a5a4305000e000000",
                "image_url": "https://consumernotebook.s3.amazonaws.com/products/www.sublimetext.com/screenshots/pythonHeroSmall.png",
                "link": "https://consumernotebook.com/sublime-text/4f4ad53a5a4305000e000000/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f4ad53a5a4305000e000000/",
                "title": "Sublime Text"
            },
            {
                "comment": "",
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.jetbrains.com/pycharm/index.html",
                "id": "4f4ad5b861e9e4000e000000",
                "image_url": "https://consumernotebook.s3.amazonaws.com/products/www.jetbrains.com/img/logo_bw.gif",
                "link": "https://consumernotebook.com/jetbrains-pycharm/4f4ad5b861e9e4000e000000/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f4ad5b861e9e4000e000000/",
                "title": "JetBrains PyCharm"
            },
            {
                "comment": "",
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//pydev.org/",
                "id": "4f4ad5d55a4c6f000d000000",
                "image_url": "https://consumernotebook.s3.amazonaws.com/products/pydev.org/images/pydev_banner2.gif",
                "link": "https://consumernotebook.com/pydev/4f4ad5d55a4c6f000d000000/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f4ad5d55a4c6f000d000000/",
                "title": "PyDev"
            },
            {
                "comment": "",
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=https%3A//store.activestate.com/komodo-ide",
                "id": "4f4bedc7776e5e000c000000",
                "image_url": "https://consumernotebook.s3.amazonaws.com/products/store.activestate.com/sites/default/files/category_pictures/box_2012_komodo_ide_7.png",
                "link": "https://consumernotebook.com/komodo-ide-7-from-activestate/4f4bedc7776e5e000c000000/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f4bedc7776e5e000c000000/",
                "title": "Komodo IDE 7 from ActiveState"
            },
            {
                "comment": "According to codeplex, VS supports both Iron Python and CPython.",
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.microsoftstore.com/store/msstore/en_US/pd/productID.216633300/topseller.true",
                "id": "4f4c298b611f84000d000000",
                "image_url": "https://consumernotebook.s3.amazonaws.com/products/dri1.img.digitalrivercontent.net/DRHM/Storefront/Company/msstore/images/software/pdp/en-US_Visual_Studio_Pro_2010_ESD_C5E-00532.jpg",
                "link": "https://consumernotebook.com/microsoft-visual-studio-2010-professional/4f4c298b611f84000d000000/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f4c298b611f84000d000000/",
                "title": "Microsoft Visual Studio 2010 Professional"
            }],
            "resource_uri": "/api/v1/lists/pydanny/complete-list-of-python-editors/",
            "slug": "complete-list-of-python-editors",
            "title": "Complete List of Python Editors",
            "url": "http://consumernotebook.com/lists/pydanny/complete-list-of-python-editors/"
        },
        {
            "created": "2012-02-25T13:24:39.212716",
            "description": "",
            "id": "500",
            "last_modified_by_user": "2012-02-25T11:59:07.083030",
            "modified": "2012-03-18T21:33:31.257813",
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
                "external_link": "http://www.amazon.com/gp/product/B0050SW8OS/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f4951976721be000e000002",
                "image_url": "http://ecx.images-amazon.com/images/I/51%2Bqo7LzBgL.jpg",
                "link": "https://consumernotebook.com/uncharted-golden-abyss/4f4951976721be000e000002/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f4951976721be000e000002/",
                "title": "Uncharted: Golden Abyss"
            },
            {
                "comment": "",
                "external_link": "http://www.amazon.com/gp/product/B006PP41Q8/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f4951ac3ad8f20012000000",
                "image_url": "http://ecx.images-amazon.com/images/I/31lvjvwfwxL.jpg",
                "link": "https://consumernotebook.com/playstation-vita-travel-pouch/4f4951ac3ad8f20012000000/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f4951ac3ad8f20012000000/",
                "title": "PlayStation Vita Travel Pouch"
            },
            {
                "comment": "",
                "external_link": "http://www.amazon.com/gp/product/B006WJ6YH6/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f4951bcdd83af000d000000",
                "image_url": "http://ecx.images-amazon.com/images/I/61UdIS4QRTL.jpg",
                "link": "https://consumernotebook.com/rayman-origins-playstation-vita-video-games/4f4951bcdd83af000d000000/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f4951bcdd83af000d000000/",
                "title": "Rayman Origins: playstation vita: Video Games"
            },
            {
                "comment": "",
                "external_link": "http://www.amazon.com/gp/product/B006VB2W08/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f4951d26721be000d000004",
                "image_url": "http://ecx.images-amazon.com/images/I/51TcmZUul6L.jpg",
                "link": "https://consumernotebook.com/lumines-electronic-symphonygames/4f4951d26721be000d000004/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f4951d26721be000d000004/",
                "title": "Lumines: Electronic SymphonyGames"
            },
            {
                "comment": "",
                "external_link": "http://www.amazon.com/gp/product/B005UDTT7C/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f4951e8dd83af000e000002",
                "image_url": "http://ecx.images-amazon.com/images/I/61VPZBc9jtL.jpg",
                "link": "https://consumernotebook.com/ultimate-marvel-vs-capcom-3-playstation-vita/4f4951e8dd83af000e000002/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f4951e8dd83af000e000002/",
                "title": "Ultimate Marvel vs Capcom 3: playstation vita"
            },
            {
                "comment": "",
                "external_link": "http://www.amazon.com/gp/product/B006JKASCK/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f49fe32251fca000e000000",
                "image_url": "http://ecx.images-amazon.com/images/I/51yVozJTUlL.jpg",
                "link": "https://consumernotebook.com/32gb-playstation-vita-memory-card/4f49fe32251fca000e000000/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f49fe32251fca000e000000/",
                "title": "32GB PlayStation Vita Memory Card"
            },
            {
                "comment": "",
                "external_link": "http://www.amazon.com/gp/product/B002I0GY9G/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f49fe4a80efee000c000000",
                "image_url": "http://ecx.images-amazon.com/images/I/516L0JC1b9L.jpg",
                "link": "https://consumernotebook.com/army-corps-of-hell/4f49fe4a80efee000c000000/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f49fe4a80efee000c000000/",
                "title": "Army Corps of Hell"
            },
            {
                "comment": "",
                "external_link": "http://www.amazon.com/gp/product/B006JKARZS/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f49fe5e58d56d000e000003",
                "image_url": "http://ecx.images-amazon.com/images/I/31lbtT45WjL.jpg",
                "link": "https://consumernotebook.com/playstation-vita-cradle-video-games/4f49fe5e58d56d000e000003/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f49fe5e58d56d000e000003/",
                "title": "PlayStation Vita Cradle: Video Games"
            },
            {
                "comment": "",
                "external_link": "http://www.amazon.com/gp/product/B0050SW93S/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f49fe75251fca000e000002",
                "image_url": "http://ecx.images-amazon.com/images/I/517T81mwtUL.jpg",
                "link": "https://consumernotebook.com/resistance-burning-skies/4f49fe75251fca000e000002/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f49fe75251fca000e000002/",
                "title": "Resistance: Burning Skies"
            },
            {
                "comment": "",
                "external_link": "http://www.amazon.com/gp/product/B006JI3Q7G/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f49fe9a251fca000c000003",
                "image_url": "http://ecx.images-amazon.com/images/I/51zm67qu-lL.jpg",
                "link": "https://consumernotebook.com/ea-sports-fifa-soccer/4f49fe9a251fca000c000003/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f49fe9a251fca000c000003/",
                "title": "EA Sports FIFA Soccer"
            },
            {
                "comment": "",
                "external_link": "http://www.amazon.com/gp/product/B006VB2W0S/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f49feaa80efee000e000000",
                "image_url": "http://ecx.images-amazon.com/images/I/51RWFClN%2B4L.jpg",
                "link": "https://consumernotebook.com/dungeon-hunter-alliance/4f49feaa80efee000e000000/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f49feaa80efee000e000000/",
                "title": "Dungeon Hunter Alliance"
            },
            {
                "comment": "",
                "external_link": "http://www.amazon.com/gp/product/B006FRNBB2/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f49feba251fca000d000000",
                "image_url": "http://ecx.images-amazon.com/images/I/61VdnLL2SPL.jpg",
                "link": "https://consumernotebook.com/touch-my-katamari/4f49feba251fca000d000000/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f49feba251fca000d000000/",
                "title": "Touch My Katamari"
            },
            {
                "comment": "",
                "external_link": "http://www.amazon.com/gp/product/B006ZPAY46/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f49fec980efee000d000000",
                "image_url": "http://ecx.images-amazon.com/images/I/61igaHsoqyL.jpg",
                "link": "https://consumernotebook.com/unit-13/4f49fec980efee000d000000/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f49fec980efee000d000000/",
                "title": "Unit 13"
            },
            {
                "comment": "",
                "external_link": "http://www.amazon.com/gp/product/B0074LJ3CE/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f49fed6251fca000d000002",
                "image_url": "http://ecx.images-amazon.com/images/I/51j21mljVPL.jpg",
                "link": "https://consumernotebook.com/mortal-kombat/4f49fed6251fca000d000002/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f49fed6251fca000d000002/",
                "title": "Mortal Kombat"
            },
            {
                "comment": "",
                "external_link": "http://www.amazon.com/gp/product/B006FRNASG/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f49feec80efee000e000002",
                "image_url": "http://ecx.images-amazon.com/images/I/51I7lgmDoTL.jpg",
                "link": "https://consumernotebook.com/shinobido-2-revenge-of-zen/4f49feec80efee000e000002/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f49feec80efee000e000002/",
                "title": "Shinobido 2: Revenge of Zen"
            },
            {
                "comment": "",
                "external_link": "http://www.amazon.com/gp/product/B0050SW33E/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f49feff58d56d000e000005",
                "image_url": "http://ecx.images-amazon.com/images/I/51qyuoQCD1L.jpg",
                "link": "https://consumernotebook.com/modnation-racers/4f49feff58d56d000e000005/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f49feff58d56d000e000005/",
                "title": "ModNation Racers"
            }],
            "resource_uri": "/api/v1/lists/pydanny/vita/",
            "slug": "vita",
            "title": "Vita",
            "url": "http://consumernotebook.com/lists/pydanny/vita/"
        },
        {
            "created": "2012-02-25T13:09:29.624082",
            "description": "",
            "id": "499",
            "last_modified_by_user": "2012-02-25T11:59:07.083030",
            "modified": "2012-03-18T21:33:31.280972",
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
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.thinkgeek.com/books/nonfiction/ec9d/%3Fpfm%3Drightcolumn_NewStuffFTW_2",
                "id": "4f494e096721be000d000002",
                "image_url": "https://consumernotebook.s3.amazonaws.com/products/www.thinkgeek.com/images/products/frontsquare/ec9d_the_manga_cookbook.jpg",
                "link": "https://consumernotebook.com/the-manga-cookbook/4f494e096721be000d000002/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f494e096721be000d000002/",
                "title": "The Manga Cookbook"
            }],
            "resource_uri": "/api/v1/lists/pydanny/kitchen-fun/",
            "slug": "kitchen-fun",
            "title": "Kitchen Fun",
            "url": "http://consumernotebook.com/lists/pydanny/kitchen-fun/"
        },
        {
            "created": "2012-02-20T00:58:29.533556",
            "description": "",
            "id": "450",
            "last_modified_by_user": "2012-02-19T17:15:31.026725",
            "modified": "2012-03-18T21:33:33.701118",
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
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.vitaminworld.com/omega-3-and-flaxseed-228/triple-omega-3-6-9-018520",
                "id": "4f420b7b758920000b000006",
                "image_url": "http://images.vitaminimages.com/vw/VF/Assets/VitaminWorld_Products/018520.jpg",
                "link": "https://consumernotebook.com/triple-omega-3-6-9-coenzyme-q10coq10-supplements/4f420b7b758920000b000006/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f420b7b758920000b000006/",
                "title": "Triple Omega 3-6-9 | Coenzyme Q10/CoQ10 Supplements"
            },
            {
                "comment": "",
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.vitaminworld.com/omega-3-and-flaxseed-228/omega-3-fish-oil-1000-mg-003835",
                "id": "4f420b93758920000b000008",
                "image_url": "http://images.vitaminimages.com/vw/VF/Assets/VitaminWorld_Products/003835.jpg",
                "link": "https://consumernotebook.com/omega-3-fish-oil-1000-mg/4f420b93758920000b000008/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f420b93758920000b000008/",
                "title": "Omega-3 Fish Oil 1000 mg"
            },
            {
                "comment": "",
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.vitaminworld.com/omega-3-and-flaxseed-228/maximum-strength-triple-omega-3-6-9-010148",
                "id": "4f420baae7615d000c00000e",
                "image_url": "http://images.vitaminimages.com/vw/VF/Assets/VitaminWorld_Products/010148.jpg",
                "link": "https://consumernotebook.com/maximum-strength-triple-omega-3-6-9/4f420baae7615d000c00000e/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f420baae7615d000c00000e/",
                "title": "Maximum Strength Triple Omega 3-6-9"
            },
            {
                "comment": "",
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.vitaminworld.com/omega-3-and-flaxseed-228/wild-salmon-oil-1000-mg-004463",
                "id": "4f420be1758920000c000006",
                "image_url": "http://images.vitaminimages.com/vw/VF/Assets/VitaminWorld_Products/004463.jpg",
                "link": "https://consumernotebook.com/wild-salmon-oil-1000-mg/4f420be1758920000c000006/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f420be1758920000c000006/",
                "title": "Wild Salmon Oil 1000 mg."
            }],
            "resource_uri": "/api/v1/lists/pydanny/health-food-and-vitamins/",
            "slug": "health-food-and-vitamins",
            "title": "Health Food and vitamins",
            "url": "http://consumernotebook.com/lists/pydanny/health-food-and-vitamins/"
        },
        {
            "created": "2012-02-18T22:14:55.262107",
            "description": "",
            "id": "438",
            "last_modified_by_user": "2012-02-18T22:09:23.437132",
            "modified": "2012-03-18T21:33:34.473370",
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
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.performancebike.com/bikes/Product_10052_10551_1094383_-1_1657509_1657508_400327",
                "id": "4f40935fefc040000a000000",
                "image_url": "http://media.performancebike.com/images/performance/products/medium/30-4207-BLG-SIDE.jpg",
                "link": "https://consumernotebook.com/2011-fuji-outland-29er-20-mountain-bike/4f40935fefc040000a000000/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f40935fefc040000a000000/",
                "title": "2011 Fuji Outland 29er 2.0 Mountain Bike"
            },
            {
                "comment": "",
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.performancebike.com/bikes/Product_10052_10551_1110572_-1_1660010_1660008_400327",
                "id": "4f409389759712000c000000",
                "image_url": "http://media.performancebike.com/images/performance/products/medium/30-8976-BLK-SIDE.jpg",
                "link": "https://consumernotebook.com/2012-diamondback-overdrive-29er-mountain-bike/4f409389759712000c000000/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f409389759712000c000000/",
                "title": "2012 Diamondback Overdrive 29er Mountain Bike"
            }],
            "resource_uri": "/api/v1/lists/pydanny/mountain-bikes/",
            "slug": "mountain-bikes",
            "title": "Mountain Bikes",
            "url": "http://consumernotebook.com/lists/pydanny/mountain-bikes/"
        },
        {
            "created": "2012-02-17T09:33:26.879452",
            "description": "This is where I list all the cycling gear I own or want to own or am evaluating.",
            "id": "428",
            "last_modified_by_user": "2012-02-17T08:20:12.277756",
            "modified": "2012-03-18T21:33:35.118906",
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
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.cleatskins.com/shop/Bikeskins%2520-%2520FullCoverageBikeskins/White",
                "id": "4f3e901fe0e026000c000001",
                "image_url": "http://www.cleatskins.com/shop/sites/default/files/imagecache/product/skins-085179%20final%20hero%20copy.jpg",
                "link": "https://consumernotebook.com/cleatskins-bikeskins-white-cleatskins/4f3e901fe0e026000c000001/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f3e901fe0e026000c000001/",
                "title": "Cleatskins Bikeskins - White | Cleatskins"
            },
            {
                "comment": "",
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.performancebike.com/bikes/Product_10052_10551_1110572_-1_1660010_1660008_400327",
                "id": "4f409389759712000c000000",
                "image_url": "http://media.performancebike.com/images/performance/products/medium/30-8976-BLK-SIDE.jpg",
                "link": "https://consumernotebook.com/2012-diamondback-overdrive-29er-mountain-bike/4f409389759712000c000000/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f409389759712000c000000/",
                "title": "2012 Diamondback Overdrive 29er Mountain Bike"
            }],
            "resource_uri": "/api/v1/lists/pydanny/bicyling/",
            "slug": "bicyling",
            "title": "Bicyling",
            "url": "http://consumernotebook.com/lists/pydanny/bicyling/"
        },
        {
            "created": "2012-02-16T11:55:24.279846",
            "description": "I need clothes and garments. The workouts are long and glorious, and I'm tired of lugging in an old travel backback.",
            "id": "425",
            "last_modified_by_user": "2012-02-18T13:56:45.549575",
            "modified": "2012-03-18T21:33:35.246908",
            "owner": {
                "avatar": "/media/avatars/pydanny/resized/80/avatars/pydanny/daniel.greenfeld.jpg",
                "coins": 122,
                "fullname": "Daniel Greenfelds",
                "score": 695,
                "username": "pydanny",
                "waitlisted": false
            },
            "products": [{
                "comment": "While it would be nice to get something that had Capoeira Batuque on it, this is a nice generic label.",
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.virtualcapoeira.com/info/accessories/pact_show/id_20420782/",
                "id": "4f3d5f48378789000b000000",
                "image_url": "http://www.virtualcapoeira.com/net/content/9291051201112819505420_300.jpg",
                "link": "https://consumernotebook.com/capoeira-cinch-pack-with-zipper-pocket/4f3d5f48378789000b000000/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f3d5f48378789000b000000/",
                "title": "Capoeira Cinch Pack with Zipper Pocket"
            },
            {
                "comment": "",
                "external_link": "http://www.amazon.com/gp/product/B00547V62U/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f3d5f88378789000b000001",
                "image_url": "http://ecx.images-amazon.com/images/I/41LP21MqZmL.jpg",
                "link": "https://consumernotebook.com/hoodie-mens-black-capoeira-color-up-sports-clothing/4f3d5f88378789000b000001/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f3d5f88378789000b000001/",
                "title": "Hoodie Mens Black \" CAPOEIRA COLOR UP \" Sports: Clothing"
            },
            {
                "comment": "",
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.virtualcapoeira.com/info/pants/pact_show/id_19386040/%3F",
                "id": "4f3d5f9b378789000c000001",
                "image_url": "http://www.virtualcapoeira.com/net/content/92910512006621233358879_300.jpg",
                "link": "https://consumernotebook.com/mens-white-training-pants-capoeira-pants-for-practicing/4f3d5f9b378789000c000001/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f3d5f9b378789000c000001/",
                "title": "Mens White Training Pants | Capoeira Pants for Practicing"
            },
            {
                "comment": "",
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.virtualcapoeira.com/info/havaianas/pact_show/id_19385982/",
                "id": "4f401e2eb5cf53000b000001",
                "image_url": "http://www.virtualcapoeira.com/net/content/92910512006510221942913_300.jpg",
                "link": "https://consumernotebook.com/brazil-havaianas/4f401e2eb5cf53000b000001/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f401e2eb5cf53000b000001/",
                "title": "Brazil Havaianas"
            },
            {
                "comment": "",
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.virtualcapoeira.com/info/atabaques/pact_show/id_19384823/",
                "id": "4f401ed75192ba000a000004",
                "image_url": "http://www.virtualcapoeira.com/net/content/92910512008121012593380_500.jpg",
                "link": "https://consumernotebook.com/atabaque-improved/4f401ed75192ba000a000004/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f401ed75192ba000a000004/",
                "title": "Atabaque - Improved!"
            },
            {
                "comment": "",
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.virtualcapoeira.com/info/pandeiros/pact_show/id_19386016/",
                "id": "4f401f00b5cf53000b000002",
                "image_url": "http://www.virtualcapoeira.com/net/content/9291051200831193154964_500.jpg",
                "link": "https://consumernotebook.com/pandeiro/4f401f00b5cf53000b000002/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f401f00b5cf53000b000002/",
                "title": "Pandeiro"
            },
            {
                "comment": "",
                "external_link": "http://www.amazon.com/gp/product/B004QITIAA/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f45afcafac4280100000000",
                "image_url": "http://ecx.images-amazon.com/images/I/51WxYLydVVL.jpg",
                "link": "https://consumernotebook.com/basic-techniques-of-capoeira/4f45afcafac4280100000000/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f45afcafac4280100000000/",
                "title": "Basic Techniques Of Capoeira"
            }],
            "resource_uri": "/api/v1/lists/pydanny/capoeira-gear/",
            "slug": "capoeira-gear",
            "title": "Capoeira Gear",
            "url": "http://consumernotebook.com/lists/pydanny/capoeira-gear/"
        },
        {
            "created": "2012-01-19T00:28:26.246811",
            "description": "These are ones with crisp technique, camera, and plot.",
            "id": "420",
            "last_modified_by_user": "2012-02-15T19:39:19.418103",
            "modified": "2012-03-18T21:33:35.399116",
            "owner": {
                "avatar": "/media/avatars/pydanny/resized/80/avatars/pydanny/daniel.greenfeld.jpg",
                "coins": 122,
                "fullname": "Daniel Greenfelds",
                "score": 695,
                "username": "pydanny",
                "waitlisted": false
            },
            "products": [{
                "comment": "Really good from a technical aspect, this traditional martial arts story is like a step back into some of the post-war films about the Sino-Japanese conflict.",
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.tkqlhce.com/click-5536662-10475872%3Furl%3Dhttp%253A%252F%252Fwww.bestbuy.com%252Fsite%252Folspage.jsp%253Fid%253D1954262%2526skuId%253D18601525%2526type%253Dproduct%2526ci_src%253D11138%2526ci_sku%253D18601525",
                "id": "4f3c0176ebae2600040000dd",
                "image_url": "http://images.bestbuy.com/BestBuy_US/images/products/1860/18601525.jpg",
                "link": "https://consumernotebook.com/ip-man-dubbed-subtitle-ac3/4f3c0176ebae2600040000dd/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f3c0176ebae2600040000dd/",
                "title": "Ip Man - Dubbed Subtitle AC3"
            },
            {
                "comment": "This is the original 1978 film with master kicker Hwang Jang Lee as the bad guy. The subtitled version is infinitely better than the dubbed, because otherwise you will miss the earth, rich Cantonese humor of the period. ",
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.jdoqocy.com/click-5536662-10475872%3Furl%3Dhttp%253A%252F%252Fwww.bestbuy.com%252Fsite%252Folspage.jsp%253Fid%253D21522%2526skuId%253D4522369%2526type%253Dproduct%2526ci_src%253D11138%2526ci_sku%253D4522369",
                "id": "4f3c0187ebae260004000140",
                "image_url": "http://images.bestbuy.com/BestBuy_US/images/products/4522/4522369.jpg",
                "link": "https://consumernotebook.com/drunken-master-widescreen-dubbed-subtitle/4f3c0187ebae260004000140/",
                "price_range": "$10-20",
                "resource_uri": "/api/v1/products/4f3c0187ebae260004000140/",
                "title": "Drunken Master - Widescreen Dubbed Subtitle"
            },
            {
                "comment": "The sequel to the first Ip Man movie, this is a really good depiction of post-war Hong Kong. The early part of the film has an embellished depiction of the sort of challenges that used to happen in martial arts communities. The later part of the movie is also pretty good, sort of like Rocky I & II but with Kung Fu vs Boxing.",
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.tkqlhce.com/click-5536662-10475872%3Furl%3Dhttp%253A%252F%252Fwww.bestbuy.com%252Fsite%252Folspage.jsp%253Fid%253D2181504%2526skuId%253D19008394%2526type%253Dproduct%2526ci_src%253D11138%2526ci_sku%253D19008394",
                "id": "4f3c018bebae26000400016f",
                "image_url": "http://images.bestbuy.com/BestBuy_US/images/products/1900/19008394.jpg",
                "link": "https://consumernotebook.com/ip-man-2-legend-of-the-grandmaster-/4f3c018bebae26000400016f/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f3c018bebae26000400016f/",
                "title": "Ip Man 2: Legend of the Grandmaster -"
            }],
            "resource_uri": "/api/v1/lists/pydanny/good-martial-arts-movies/",
            "slug": "good-martial-arts-movies",
            "title": "Good Martial Arts movies",
            "url": "http://consumernotebook.com/lists/pydanny/good-martial-arts-movies/"
        },
        {
            "created": "2012-01-17T16:17:28.595236",
            "description": "I love Python but I'm doing a lot of Javascript these days. Either in JQuery or MongoDB. These are the books that I live by in my day-to-day efforts as a developer.",
            "id": "418",
            "last_modified_by_user": "2012-02-15T19:39:46.183310",
            "modified": "2012-03-18T21:33:35.533323",
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
                "external_link": "http://www.amazon.com/gp/product/0596517742/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f3c0164ebae260004000040",
                "image_url": "http://ecx.images-amazon.com/images/I/51YIYr01vsL.jpg",
                "link": "https://consumernotebook.com/javascript-the-good-parts/4f3c0164ebae260004000040/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f3c0164ebae260004000040/",
                "title": "JavaScript: The Good Parts"
            },
            {
                "comment": "",
                "external_link": "http://www.amazon.com/gp/product/193398869X/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f3c0192ebae260004000186",
                "image_url": "http://ecx.images-amazon.com/images/I/51jbPsZnqhL.jpg",
                "link": "https://consumernotebook.com/secrets-of-the-javascript-ninja/4f3c0192ebae260004000186/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f3c0192ebae260004000186/",
                "title": "Secrets of the JavaScript Ninja"
            }],
            "resource_uri": "/api/v1/lists/pydanny/must-have-javascript-books/",
            "slug": "must-have-javascript-books",
            "title": "Must have Javascript books",
            "url": "http://consumernotebook.com/lists/pydanny/must-have-javascript-books/"
        },
        {
            "created": "2012-01-06T20:50:43.350547",
            "description": "Here is a straight-forward list of books I want to read.",
            "id": "396",
            "last_modified_by_user": "2012-02-27T23:25:01.052168",
            "modified": "2012-03-18T21:33:35.905302",
            "owner": {
                "avatar": "/media/avatars/pydanny/resized/80/avatars/pydanny/daniel.greenfeld.jpg",
                "coins": 122,
                "fullname": "Daniel Greenfelds",
                "score": 695,
                "username": "pydanny",
                "waitlisted": false
            },
            "products": [{
                "comment": "Numpy book to help me get deep into this amazing library? Yes please!",
                "external_link": "http://www.amazon.com/gp/product/1849515301/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f3c0163ebae26000400002d",
                "image_url": "http://ecx.images-amazon.com/images/I/51o0XqA%2BsLL.jpg",
                "link": "https://consumernotebook.com/numpy-15-beginners-guide/4f3c0163ebae26000400002d/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f3c0163ebae26000400002d/",
                "title": "NumPy 1.5 Beginner's Guide"
            },
            {
                "comment": "I want to learn about licensing and here we go.",
                "external_link": "http://www.amazon.com/gp/product/0596517963/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f3c0164ebae260004000054",
                "image_url": "http://ecx.images-amazon.com/images/I/51Wbp2dbB9L.jpg",
                "link": "https://consumernotebook.com/intellectual-property-and-open-source-a-practical-guide-to-protecting-code/4f3c0164ebae260004000054/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f3c0164ebae260004000054/",
                "title": "Intellectual Property and Open Source: A Practical Guide to Protecting Code"
            },
            {
                "comment": "Design principals that may turn out to be useful",
                "external_link": "http://www.amazon.com/gp/product/1119998956/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f3c016aebae26000400009a",
                "image_url": "http://ecx.images-amazon.com/images/I/51SiSPTX2FL.jpg",
                "link": "https://consumernotebook.com/design-for-hackers-reverse-engineering-beauty/4f3c016aebae26000400009a/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f3c016aebae26000400009a/",
                "title": "Design for Hackers: Reverse Engineering Beauty"
            },
            {
                "comment": "Hard to find but an absolute classic. I kick myself for not buying it in the past when I had the chance.",
                "external_link": "http://www.amazon.com/gp/product/0804817162/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f3c016aebae2600040000aa",
                "image_url": "http://ecx.images-amazon.com/images/I/51zESeeKbEL.jpg",
                "link": "https://consumernotebook.com/the-weapons-and-fighting-arts-of-indonesia/4f3c016aebae2600040000aa/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f3c016aebae2600040000aa/",
                "title": "The Weapons and Fighting Arts of Indonesia"
            },
            {
                "comment": "Steve White and David Weber have an interesting science fiction series and here the former continues to the saga alone. I wish this were on Kindle but here is the paperback for good measure.",
                "external_link": "http://www.amazon.com/gp/product/1416555617/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f3c0176ebae2600040000e1",
                "image_url": "http://ecx.images-amazon.com/images/I/515VlhmCUML.jpg",
                "link": "https://consumernotebook.com/exodus-starfire-bk-5/4f3c0176ebae2600040000e1/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f3c0176ebae2600040000e1/",
                "title": "Exodus (Starfire, Bk. 5)"
            },
            {
                "comment": "The follow-up to Exodus by Steve White, this is another paperback Science Fiction book I would love to read.",
                "external_link": "http://www.amazon.com/gp/product/1439134332/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f3c0176ebae2600040000e5",
                "image_url": "http://ecx.images-amazon.com/images/I/51mmwkUYj9L.jpg",
                "link": "https://consumernotebook.com/extremis-na-starfire/4f3c0176ebae2600040000e5/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f3c0176ebae2600040000e5/",
                "title": "Extremis: N/A (Starfire)"
            },
            {
                "comment": "Wondering if this is good. It's all over the place so maybe I'll give it a try.",
                "external_link": "http://www.amazon.com/gp/product/B0015DROBO/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f3c017cebae26000400012b",
                "image_url": "http://ecx.images-amazon.com/images/I/511x0O8%2B5SL.jpg",
                "link": "https://consumernotebook.com/the-girl-with-the-dragon-tattoo-millennium-trilogy/4f3c017cebae26000400012b/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f3c017cebae26000400012b/",
                "title": "The Girl with the Dragon Tattoo (Millennium Trilogy)"
            },
            {
                "comment": "KIndle version of Van Lindburgh's critical work on intellectual property.",
                "external_link": "http://www.amazon.com/gp/product/B0043D2E3Q/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f3c019debae2600040001a8",
                "image_url": "http://ecx.images-amazon.com/images/I/51mP6v3qllL.jpg",
                "link": "https://consumernotebook.com/intellectual-property-and-open-source-a-practical-guide-to-protecting-code/4f3c019debae2600040001a8/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f3c019debae2600040001a8/",
                "title": "Intellectual Property and Open Source: A Practical Guide to Protecting Code"
            },
            {
                "comment": "By Heresies Distressed picks up exactly at the end of Book 2 of the safehold series. As the reformation gets into swing, the world leaps into turmoil.",
                "external_link": "http://www.amazon.com/gp/product/B002LATV2K/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f3c019eebae2600040001bb",
                "image_url": "http://ecx.images-amazon.com/images/I/51PKqNsiHPL.jpg",
                "link": "https://consumernotebook.com/by-heresies-distressed/4f3c019eebae2600040001bb/",
                "price_range": "$0-10",
                "resource_uri": "/api/v1/products/4f3c019eebae2600040001bb/",
                "title": "By Heresies Distressed"
            },
            {
                "comment": "",
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.packtpub.com/numpy-1-5-using-real-world-examples-beginners-guide/book%23author",
                "id": "4f44f78e358859000b00000b",
                "image_url": "https://www.packtpub.com/sites/default/files/imagecache/productview_ebook/5306OS_NumPy%201.5_FrontCover.jpg",
                "link": "https://consumernotebook.com/numpy-15-beginners-guide-packt-publishing-technical-it-book-and-ebook-store/4f44f78e358859000b00000b/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f44f78e358859000b00000b/",
                "title": "NumPy 1.5 Beginner's Guide | Packt Publishing Technical & IT Book and eBook Store"
            },
            {
                "comment": "",
                "external_link": "http://www.amazon.com/gp/product/3540739157/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f44f8565602c3000a000003",
                "image_url": "http://ecx.images-amazon.com/images/I/41N6MyO%2BIIL.jpg",
                "link": "https://consumernotebook.com/python-scripting-for-computational-science-hans-petter-langtangen/4f44f8565602c3000a000003/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f44f8565602c3000a000003/",
                "title": "Python Scripting for Computational Science  Hans Petter Langtangen"
            },
            {
                "comment": "",
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.packtpub.com/matplotlib-python-development/book",
                "id": "4f44f92f3b0a04000c000004",
                "image_url": "https://www.packtpub.com/sites/default/files/imagecache/productview_ebook/bookimages/4947_MockupCover.jpg",
                "link": "https://consumernotebook.com/matplotlib-for-python-developers-packt-publishing-technical-it-book-and-ebook-store/4f44f92f3b0a04000c000004/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f44f92f3b0a04000c000004/",
                "title": "Matplotlib for Python Developers | Packt Publishing Technical & IT Book and eBook Store"
            },
            {
                "comment": "",
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.tramy.us/",
                "id": "4f44f9d65602c3000c000009",
                "image_url": "http://www.tramy.us/setfree_small.png",
                "link": "https://consumernotebook.com/guide-to-numpy-travis-e-oliphant/4f44f9d65602c3000c000009/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f44f9d65602c3000c000009/",
                "title": "Guide to Numpy Travis E. Oliphant"
            },
            {
                "comment": "",
                "external_link": "http://www.amazon.com/gp/product/1430218436/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f4501af3b0a04000a000008",
                "image_url": "http://ecx.images-amazon.com/images/I/51ww9Itv0RL.jpg",
                "link": "https://consumernotebook.com/beginning-python-visualization-crafting-visual-transformation/4f4501af3b0a04000a000008/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f4501af3b0a04000a000008/",
                "title": "Beginning Python Visualization: Crafting Visual Transformation"
            },
            {
                "comment": "",
                "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.thinkgeek.com/books/nonfiction/ec9d/%3Fpfm%3Drightcolumn_NewStuffFTW_2",
                "id": "4f494e096721be000d000002",
                "image_url": "https://consumernotebook.s3.amazonaws.com/products/www.thinkgeek.com/images/products/frontsquare/ec9d_the_manga_cookbook.jpg",
                "link": "https://consumernotebook.com/the-manga-cookbook/4f494e096721be000d000002/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f494e096721be000d000002/",
                "title": "The Manga Cookbook"
            },
            {
                "comment": "",
                "external_link": "http://www.amazon.com/gp/product/0316007625/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f49b7c3feac66000d000000",
                "image_url": "http://ecx.images-amazon.com/images/I/51ycgh845CL.jpg",
                "link": "https://consumernotebook.com/shark-vs-train-by-chris-barton-tom-lichtenheld/4f49b7c3feac66000d000000/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f49b7c3feac66000d000000/",
                "title": "Shark vs. Train by Chris Barton, Tom Lichtenheld"
            },
            {
                "comment": "",
                "external_link": "http://www.amazon.com/gp/product/0399526145/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f5054f57eb9f6000c000000",
                "image_url": "http://ecx.images-amazon.com/images/I/51xd5JLUbDL.jpg",
                "link": "https://consumernotebook.com/the-7-powers-of-questions-secrets-to-successful-communication-in-life-and-at-work-by-dorothy-leeds/4f5054f57eb9f6000c000000/",
                "price_range": "$20-50",
                "resource_uri": "/api/v1/products/4f5054f57eb9f6000c000000/",
                "title": "The 7 Powers of Questions: Secrets to Successful Communication in Life and at Work by Dorothy Leeds"
            },
            {
                "comment": "Copernicus changed the world with this book.",
                "external_link": "http://www.amazon.com/gp/product/1573920355/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f53dc64fe40db000e000000",
                "image_url": "http://ecx.images-amazon.com/images/I/41UVdLKeROL.jpg",
                "link": "https://consumernotebook.com/on-the-revolutions-of-heavenly-spheres-by-nicolaus-copernicus-books/4f53dc64fe40db000e000000/",
                "price_range": "$10-20",
                "resource_uri": "/api/v1/products/4f53dc64fe40db000e000000/",
                "title": "On the Revolutions of Heavenly Spheres by Nicolaus Copernicus: Books"
            },
            {
                "comment": "I've read this book a few times, but I just want this nice collector's version.",
                "external_link": "http://www.amazon.com/gp/product/4770028016/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f5811d5a2fb42000e000000",
                "image_url": "http://ecx.images-amazon.com/images/I/51FIg2hszaL.jpg",
                "link": "https://consumernotebook.com/the-book-of-five-rings-bushido-the-way-of-the-warrior-9784770028013-miyamoto-musashi-william/4f5811d5a2fb42000e000000/",
                "price_range": "$50-100",
                "resource_uri": "/api/v1/products/4f5811d5a2fb42000e000000/",
                "title": "The Book of Five Rings (Bushido--The Way of the Warrior) (9784770028013): Miyamoto Musashi, William "
            },
            {
                "comment": "I really like Scalzi's \"Old Man\" universe. This is stories from the point of view of Jane Sagan.",
                "external_link": "http://www.amazon.com/gp/product/B005OTDQQ2/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f650c89931314000d000000",
                "image_url": "http://ecx.images-amazon.com/images/I/51vvGdFBs1L.jpg",
                "link": "https://consumernotebook.com/the-sagan-diary-ebook-john-scalzi-kindle-store/4f650c89931314000d000000/",
                "price_range": "$0-10",
                "resource_uri": "/api/v1/products/4f650c89931314000d000000/",
                "title": "The Sagan Diary eBook: John Scalzi: Kindle Store"
            },
            {
                "comment": "",
                "external_link": "http://www.amazon.com/gp/product/B005OTEEEA/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f657b759007d7000e000002",
                "image_url": "http://ecx.images-amazon.com/images/I/51CuKsKGF8L.jpg",
                "link": "https://consumernotebook.com/questions-for-a-soldier-ebook-john-scalzi/4f657b759007d7000e000002/",
                "price_range": "$0-10",
                "resource_uri": "/api/v1/products/4f657b759007d7000e000002/",
                "title": "Questions for a Soldier eBook: John Scalzi"
            }],
            "resource_uri": "/api/v1/lists/pydanny/book-wishlist/",
            "slug": "book-wishlist",
            "title": "Book wishlist",
            "url": "http://consumernotebook.com/lists/pydanny/book-wishlist/"
        },
        {
            "created": "2012-01-04T10:11:03.055199",
            "description": "These are pieces I want to have in my house.",
            "id": "381",
            "last_modified_by_user": "2012-01-04T17:00:06.062991",
            "modified": "2012-03-18T21:33:36.544364",
            "owner": {
                "avatar": "/media/avatars/pydanny/resized/80/avatars/pydanny/daniel.greenfeld.jpg",
                "coins": 122,
                "fullname": "Daniel Greenfelds",
                "score": 695,
                "username": "pydanny",
                "waitlisted": false
            },
            "products": [{
                "comment": "An Elephant table would go well with the Zebra Accent chair.",
                "external_link": "http://www.amazon.com/gp/product/B001AQ6GJW/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f3c017debae26000400013b",
                "image_url": "http://ecx.images-amazon.com/images/I/41ZD%2BE7s9OL.jpg",
                "link": "https://consumernotebook.com/twos-company-elephant-side-table-ceramic/4f3c017debae26000400013b/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f3c017debae26000400013b/",
                "title": "Two's Company Elephant Side Table Ceramic"
            },
            {
                "comment": "This chair would look great in a room with an indoor pool full of lovely dappled sunlight coming through the windows.",
                "external_link": "http://www.amazon.com/gp/product/B005XEHTKM/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f3c01a9ebae260004000245",
                "image_url": "http://ecx.images-amazon.com/images/I/41xhGQ2NoQL.jpg",
                "link": "https://consumernotebook.com/deco-zebra-accent-chair/4f3c01a9ebae260004000245/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f3c01a9ebae260004000245/",
                "title": "Deco Zebra Accent Chair"
            },
            {
                "comment": "need a new chair",
                "external_link": "http://www.amazon.com/gp/product/B00166DR9S/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f5a7c07204d33000c000001",
                "image_url": "http://ecx.images-amazon.com/images/I/4158fFJJcUL.jpg",
                "link": "https://consumernotebook.com/boss-black-leatherplus-executive-chair/4f5a7c07204d33000c000001/",
                "price_range": "$100-200",
                "resource_uri": "/api/v1/products/4f5a7c07204d33000c000001/",
                "title": "Boss Black LeatherPlus Executive Chair"
            },
            {
                "comment": "Yet another chair.",
                "external_link": "http://www.amazon.com/gp/product/B002ZDUDV6/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f5a85d8310cb0000c000002",
                "image_url": "http://ecx.images-amazon.com/images/I/312qZgDBpML.jpg",
                "link": "https://consumernotebook.com/flash-furniture-black-leather-office-chair-go-7194b-bk-gg-office-products/4f5a85d8310cb0000c000002/",
                "price_range": "$100-200",
                "resource_uri": "/api/v1/products/4f5a85d8310cb0000c000002/",
                "title": "Flash furniture Black Leather Office Chair, GO-7194B-BK-GG: Office Products"
            }],
            "resource_uri": "/api/v1/lists/pydanny/furniture-wishlist/",
            "slug": "furniture-wishlist",
            "title": "Furniture Wishlist",
            "url": "http://consumernotebook.com/lists/pydanny/furniture-wishlist/"
        },
        {
            "created": "2012-01-03T09:07:19.577826",
            "description": "I love documentaries!",
            "id": "378",
            "last_modified_by_user": "2012-01-03T23:35:38.095761",
            "modified": "2012-03-18T21:33:36.755567",
            "owner": {
                "avatar": "/media/avatars/pydanny/resized/80/avatars/pydanny/daniel.greenfeld.jpg",
                "coins": 122,
                "fullname": "Daniel Greenfelds",
                "score": 695,
                "username": "pydanny",
                "waitlisted": false
            },
            "products": [{
                "comment": "The story of how Capoeira came to Switzerland. Not sure if it is any good but it seems interesting.",
                "external_link": "http://www.amazon.com/gp/product/B000FGG5GC/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f3c018bebae26000400016a",
                "image_url": "http://ecx.images-amazon.com/images/I/51CdGyy0zsL.jpg",
                "link": "https://consumernotebook.com/capoeira/4f3c018bebae26000400016a/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f3c018bebae26000400016a/",
                "title": "Capoeira"
            },
            {
                "comment": "My favorite Dinosaur documentary",
                "external_link": "http://www.amazon.com/gp/product/B000GTJSFS/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f3c019febae2600040001d2",
                "image_url": "http://ecx.images-amazon.com/images/I/515caNGeHyL.jpg",
                "link": "https://consumernotebook.com/walking-with-dinosaurs/4f3c019febae2600040001d2/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f3c019febae2600040001d2/",
                "title": "Walking with Dinosaurs"
            },
            {
                "comment": "David A talking about planet Earth!",
                "external_link": "http://www.amazon.com/gp/product/B000MRAAJM/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f3c01a9ebae26000400023b",
                "image_url": "http://ecx.images-amazon.com/images/I/51vOcFKASRL.jpg",
                "link": "https://consumernotebook.com/planet-earth-the-complete-bbc-series-blu-ray/4f3c01a9ebae26000400023b/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f3c01a9ebae26000400023b/",
                "title": "Planet Earth: The Complete BBC Series [Blu-ray]"
            },
            {
                "comment": "More terrifying than any horror movie because this is the real world.",
                "external_link": "http://www.amazon.com/gp/product/B004HFKPOK/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f3c01afebae26000400027d",
                "image_url": "http://ecx.images-amazon.com/images/I/515HnSnQbeL.jpg",
                "link": "https://consumernotebook.com/inside-north-korea/4f3c01afebae26000400027d/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f3c01afebae26000400027d/",
                "title": "Inside North Korea"
            }],
            "resource_uri": "/api/v1/lists/pydanny/documentaries/",
            "slug": "documentaries",
            "title": "Documentaries",
            "url": "http://consumernotebook.com/lists/pydanny/documentaries/"
        },
        {
            "created": "2011-12-29T22:50:57.348589",
            "description": "We built Consumer Notebook with Django as one of the components. Here are a set of references that are available for study.",
            "id": "363",
            "last_modified_by_user": "2011-12-29T23:04:00.254225",
            "modified": "2012-03-18T21:33:37.156842",
            "owner": {
                "avatar": "/media/avatars/pydanny/resized/80/avatars/pydanny/daniel.greenfeld.jpg",
                "coins": 122,
                "fullname": "Daniel Greenfelds",
                "score": 695,
                "username": "pydanny",
                "waitlisted": false
            },
            "products": [{
                "comment": "Marty Alchin's book is AMAZING. This won't just make your Django skills better, it will make your Python and programming skills jump in prowess. If you get any book in this list, get this one!!!",
                "external_link": "http://www.amazon.com/gp/product/1430210478/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f3c0164ebae260004000043",
                "image_url": "http://ecx.images-amazon.com/images/I/41Ry%2BLUNkQL.jpg",
                "link": "https://consumernotebook.com/pro-django-experts-voice-in-web-development/4f3c0164ebae260004000043/",
                "price_range": "$20-50",
                "resource_uri": "/api/v1/products/4f3c0164ebae260004000043/",
                "title": "Pro Django (Expert's Voice in Web Development)"
            },
            {
                "comment": "A bit dated, but still quite handy. I honed much of my Django skills on an earlier version of this book.",
                "external_link": "http://www.amazon.com/gp/product/143021936X/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f3c0168ebae260004000070",
                "image_url": "http://ecx.images-amazon.com/images/I/5198kKFjb2L.jpg",
                "link": "https://consumernotebook.com/the-definitive-guide-to-django-web-development-done-right/4f3c0168ebae260004000070/",
                "price_range": "$20-50",
                "resource_uri": "/api/v1/products/4f3c0168ebae260004000070/",
                "title": "The Definitive Guide to Django: Web Development Done Right"
            },
            {
                "comment": "This books is terrible. The code is broken. Don't buy it!",
                "external_link": "http://www.amazon.com/gp/product/1847197000/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f3c0177ebae260004000100",
                "image_url": "http://ecx.images-amazon.com/images/I/41xUMvA8nUL.jpg",
                "link": "https://consumernotebook.com/django-12-e-commerce/4f3c0177ebae260004000100/",
                "price_range": "$20-50",
                "resource_uri": "/api/v1/products/4f3c0177ebae260004000100/",
                "title": "Django 1.2 e-commerce"
            },
            {
                "comment": "Wesley Chun is a hero of mine, and Jeff Forcier is the guy behind Fabric. Together along with Paul Bissex they deliver a serious book for experienced Python and Django developers. However, I think this book will be hard for incoming developers.",
                "external_link": "http://www.amazon.com/gp/product/0132356139/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f3c0188ebae26000400014e",
                "image_url": "http://ecx.images-amazon.com/images/I/41c1QK1THKL.jpg",
                "link": "https://consumernotebook.com/python-web-development-with-django/4f3c0188ebae26000400014e/",
                "price_range": "$20-50",
                "resource_uri": "/api/v1/products/4f3c0188ebae26000400014e/",
                "title": "Python Web Development with Django"
            },
            {
                "comment": "I have some concerns that this is using the old local_settings.py method of controlling domain specific settings. Nevertheless, it's good to see more people stepping into the role of documenters.",
                "external_link": "http://www.amazon.com/gp/product/B006OYO9SK/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f3c018aebae26000400015c",
                "image_url": "http://ecx.images-amazon.com/images/I/312kliN4qdL.jpg",
                "link": "https://consumernotebook.com/django-design-patterns/4f3c018aebae26000400015c/",
                "price_range": "$20-50",
                "resource_uri": "/api/v1/products/4f3c018aebae26000400015c/",
                "title": "Django Design Patterns"
            },
            {
                "comment": "Karen Tracey is a Django core developer and is a powerful authority on testing. This book is another handy reference for any serious Django developer.",
                "external_link": "http://www.amazon.com/gp/product/1847197566/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f3c019febae2600040001d0",
                "image_url": "http://ecx.images-amazon.com/images/I/41A0xBtW5PL.jpg",
                "link": "https://consumernotebook.com/django-11-testing-and-debugging/4f3c019febae2600040001d0/",
                "price_range": "$20-50",
                "resource_uri": "/api/v1/products/4f3c019febae2600040001d0/",
                "title": "Django 1.1 Testing and Debugging"
            },
            {
                "comment": "Really good book for getting bootstrapped into Django. ",
                "external_link": "http://www.amazon.com/gp/product/1847196780/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f3c01aaebae260004000258",
                "image_url": "http://ecx.images-amazon.com/images/I/511QYiLPJbL.jpg",
                "link": "https://consumernotebook.com/django-10-website-development/4f3c01aaebae260004000258/",
                "price_range": "$20-50",
                "resource_uri": "/api/v1/products/4f3c01aaebae260004000258/",
                "title": "Django 1.0 Website Development"
            }],
            "resource_uri": "/api/v1/lists/pydanny/django-books/",
            "slug": "django-books",
            "title": "Django Books",
            "url": "http://consumernotebook.com/lists/pydanny/django-books/"
        },
        {
            "created": "2011-12-28T23:26:51.995378",
            "description": "How can anyone go wrong with Lego based video games?",
            "id": "354",
            "last_modified_by_user": "2011-12-28T23:29:55.634628",
            "modified": "2012-03-18T21:33:37.610790",
            "owner": {
                "avatar": "/media/avatars/pydanny/resized/80/avatars/pydanny/daniel.greenfeld.jpg",
                "coins": 122,
                "fullname": "Daniel Greenfelds",
                "score": 695,
                "username": "pydanny",
                "waitlisted": false
            },
            "products": [{
                "comment": "Cue dramatic pulp action and pulse-pouding music when you play as Indiana Jones in a world of Legos.",
                "external_link": "http://www.amazon.com/gp/product/B0010YOQJQ/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f3c0177ebae2600040000f5",
                "image_url": "http://ecx.images-amazon.com/images/I/51QEGrxvkcL.jpg",
                "link": "https://consumernotebook.com/lego-indiana-jones-the-original-adventures/4f3c0177ebae2600040000f5/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f3c0177ebae2600040000f5/",
                "title": "Lego Indiana Jones: The Original Adventures"
            },
            {
                "comment": "Fight injustice as the Batman in a Lego version of Gotham city!",
                "external_link": "http://www.amazon.com/gp/product/B000ZKBJY6/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f3c019febae2600040001ce",
                "image_url": "http://ecx.images-amazon.com/images/I/517zan%2Bv3eL.jpg",
                "link": "https://consumernotebook.com/lego-batman/4f3c019febae2600040001ce/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f3c019febae2600040001ce/",
                "title": "Lego Batman"
            },
            {
                "comment": "Play through the original Star Wars series as Lego characters!",
                "external_link": "http://www.amazon.com/gp/product/B000G7X0AO/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f3c019febae2600040001e0",
                "image_url": "http://ecx.images-amazon.com/images/I/51I5gVRtCWL.jpg",
                "link": "https://consumernotebook.com/lego-star-wars-ii-the-original-trilogy/4f3c019febae2600040001e0/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f3c019febae2600040001e0/",
                "title": "Lego Star Wars II: The Original Trilogy"
            },
            {
                "comment": "Battle the nefarious robot armies as brave jedi!",
                "external_link": "http://www.amazon.com/gp/product/B0037UCTCW/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f3c01adebae260004000266",
                "image_url": "http://ecx.images-amazon.com/images/I/514B%2Bw86lIL.jpg",
                "link": "https://consumernotebook.com/lego-star-wars-iii-the-clone-wars/4f3c01adebae260004000266/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f3c01adebae260004000266/",
                "title": "LEGO Star Wars III The Clone Wars"
            }],
            "resource_uri": "/api/v1/lists/pydanny/lego-video-games/",
            "slug": "lego-video-games",
            "title": "Lego Video Games",
            "url": "http://consumernotebook.com/lists/pydanny/lego-video-games/"
        },
        {
            "created": "2011-12-27T18:18:06.972592",
            "description": "This is a list about Zombies. Books, games, movies, and more!",
            "id": "342",
            "last_modified_by_user": "2012-02-15T23:44:57.683994",
            "modified": "2012-03-18T21:33:37.691888",
            "owner": {
                "avatar": "/media/avatars/pydanny/resized/80/avatars/pydanny/daniel.greenfeld.jpg",
                "coins": 122,
                "fullname": "Daniel Greenfelds",
                "score": 695,
                "username": "pydanny",
                "waitlisted": false
            },
            "products": [{
                "comment": "I received this as a birthday present in July of 2011 from Grant and Sophia Viklund.",
                "external_link": "http://www.amazon.com/gp/product/1400049628/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f3c016aebae2600040000b4",
                "image_url": "http://ecx.images-amazon.com/images/I/51kfZ29lrGL.jpg",
                "link": "https://consumernotebook.com/the-zombie-survival-guide-complete-protection-from-the-living-dead/4f3c016aebae2600040000b4/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f3c016aebae2600040000b4/",
                "title": "The Zombie Survival Guide: Complete Protection from the Living Dead"
            },
            {
                "comment": "This is supposed to a fun, silly game that is easy to learn and play.",
                "external_link": "http://www.amazon.com/gp/product/B003IKMR0U/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f3c017aebae260004000116",
                "image_url": "http://ecx.images-amazon.com/images/I/51S48Jj28IL.jpg",
                "link": "https://consumernotebook.com/zombie-dice/4f3c017aebae260004000116/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f3c017aebae260004000116/",
                "title": "Zombie Dice"
            },
            {
                "comment": "In case you get turned into a Zombie, this is a guide as to what you should be doing!",
                "external_link": "http://www.amazon.com/gp/product/1569763429/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f3c0188ebae260004000142",
                "image_url": "http://ecx.images-amazon.com/images/I/51gQHCAlRaL.jpg",
                "link": "https://consumernotebook.com/so-now-youre-a-zombie-a-handbook-for-the-newly-undead-humour/4f3c0188ebae260004000142/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f3c0188ebae260004000142/",
                "title": "So Now You're a Zombie: A Handbook for the Newly Undead (Humour)"
            },
            {
                "comment": "I love how Max Brooks channels Studs Turkel in writing about the great Zombie war and how mankind was chased into near extinction and yet manages to survive against the odds.",
                "external_link": "http://www.amazon.com/gp/product/B000JMKQX0/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f3c019eebae2600040001cc",
                "image_url": "http://ecx.images-amazon.com/images/I/51d2Jv0LZTL.jpg",
                "link": "https://consumernotebook.com/world-war-z-an-oral-history-of-the-zombie-war/4f3c019eebae2600040001cc/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f3c019eebae2600040001cc/",
                "title": "World War Z: An Oral History of the Zombie War"
            },
            {
                "comment": "",
                "external_link": "http://www.amazon.com/gp/product/B0018OIK0E/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f3cb43a5e73c2000c000000",
                "image_url": "http://ecx.images-amazon.com/images/I/51bRrMdvLtL.jpg",
                "link": "https://consumernotebook.com/shaun-of-the-dead/4f3cb43a5e73c2000c000000/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f3cb43a5e73c2000c000000/",
                "title": "Shaun of the Dead"
            },
            {
                "comment": "",
                "external_link": "http://www.amazon.com/gp/product/B0030B624E/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f3cb47a5e73c2000b000000",
                "image_url": "http://ecx.images-amazon.com/images/I/51NgH8TbMtL.jpg",
                "link": "https://consumernotebook.com/zombieland-amazon-instant-video/4f3cb47a5e73c2000b000000/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f3cb47a5e73c2000b000000/",
                "title": "Zombieland: Amazon Instant Video"
            }],
            "resource_uri": "/api/v1/lists/pydanny/zombies/",
            "slug": "zombies",
            "title": "Zombies",
            "url": "http://consumernotebook.com/lists/pydanny/zombies/"
        },
        {
            "created": "2011-12-26T11:25:19.509885",
            "description": "These are board games where instead of competing together you tend to work together to win a common goal.",
            "id": "337",
            "last_modified_by_user": "2011-12-28T15:21:44.191176",
            "modified": "2012-03-18T21:33:37.815438",
            "owner": {
                "avatar": "/media/avatars/pydanny/resized/80/avatars/pydanny/daniel.greenfeld.jpg",
                "coins": 122,
                "fullname": "Daniel Greenfelds",
                "score": 695,
                "username": "pydanny",
                "waitlisted": false
            },
            "products": [{
                "comment": "You and the other players are racing to rescue archeological treasures from a sinking island. Work together to save these pieces or sink to a watery doom!",
                "external_link": "http://www.amazon.com/gp/product/B003D7F4YY/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f3c0161ebae26000400000d",
                "image_url": "http://ecx.images-amazon.com/images/I/51UmKMROcNL.jpg",
                "link": "https://consumernotebook.com/forbidden-island/4f3c0161ebae26000400000d/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f3c0161ebae26000400000d/",
                "title": "Forbidden Island"
            },
            {
                "comment": "Work together to save the remainder of humanity from the Cylons. Unfortunately one player is a Cylon agent and rooting that person out is the only way to save humanity.",
                "external_link": "http://www.amazon.com/gp/product/1589944607/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f3c0164ebae260004000053",
                "image_url": "http://ecx.images-amazon.com/images/I/41MEFeBm9XL.jpg",
                "link": "https://consumernotebook.com/battlestar-galactica/4f3c0164ebae260004000053/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f3c0164ebae260004000053/",
                "title": "Battlestar Galactica"
            },
            {
                "comment": "Cooperate with the other players to find the cures to 4 terrible plagues or humanity perishes into the night.",
                "external_link": "http://www.amazon.com/gp/product/B0013OBXG2/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f3c016aebae2600040000ad",
                "image_url": "http://ecx.images-amazon.com/images/I/51Zt7Dh94zL.jpg",
                "link": "https://consumernotebook.com/pandemic/4f3c016aebae2600040000ad/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f3c016aebae2600040000ad/",
                "title": "Pandemic"
            },
            {
                "comment": "Gears of War is a very popular video game franchise, and in this board game you and the other players make up a squad trying to accomplish missions against the locusts.",
                "external_link": "http://www.amazon.com/gp/product/1616611693/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f3c0188ebae26000400014b",
                "image_url": "http://ecx.images-amazon.com/images/I/51TPRDWORcL.jpg",
                "link": "https://consumernotebook.com/gears-of-war-the-board-game/4f3c0188ebae26000400014b/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f3c0188ebae26000400014b/",
                "title": "Gears Of War The Board Game"
            },
            {
                "comment": "Imagine playing as knights of King Arthur's Court; which means righting wrongs and correcting injustices, all while trying to keep the fall of the kingdom at bay. In larger games one player becomes the betrayer and tension is added to the play as rooting out this person becomes more and more important. Tons of fun!",
                "external_link": "http://www.amazon.com/gp/product/0975277383/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f3c019eebae2600040001c7",
                "image_url": "http://ecx.images-amazon.com/images/I/61X8ILdd7qL.jpg",
                "link": "https://consumernotebook.com/shadows-over-camelot/4f3c019eebae2600040001c7/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f3c019eebae2600040001c7/",
                "title": "Shadows Over Camelot"
            }],
            "resource_uri": "/api/v1/lists/pydanny/cooperative-board-games/",
            "slug": "cooperative-board-games",
            "title": "Cooperative Board Games",
            "url": "http://consumernotebook.com/lists/pydanny/cooperative-board-games/"
        },
        {
            "created": "2011-12-23T14:02:36.077775",
            "description": "These are all one-use items that may not be practical all the time, but they are fun to have around for special occasions.",
            "id": "324",
            "last_modified_by_user": "2012-01-05T11:14:54.613236",
            "modified": "2012-03-18T21:33:38.022526",
            "owner": {
                "avatar": "/media/avatars/pydanny/resized/80/avatars/pydanny/daniel.greenfeld.jpg",
                "coins": 122,
                "fullname": "Daniel Greenfelds",
                "score": 695,
                "username": "pydanny",
                "waitlisted": false
            },
            "products": [{
                "comment": "Fondue is fun and yummy.",
                "external_link": "http://www.amazon.com/gp/product/B00018RR48/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f3c0163ebae260004000027",
                "image_url": "http://ecx.images-amazon.com/images/I/41HAPjD%2BZXL.jpg",
                "link": "https://consumernotebook.com/cuisinart-cfo-3ss-electric-fondue-maker/4f3c0163ebae260004000027/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f3c0163ebae260004000027/",
                "title": "Cuisinart CFO-3SS Electric Fondue Maker"
            },
            {
                "comment": "I love dehydrated fruit. This seems like such a wonderful thing. Can you dehydrate a person with not much of a brain?",
                "external_link": "http://www.amazon.com/gp/product/B000FFVJ3C/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f3c0164ebae26000400003b",
                "image_url": "http://ecx.images-amazon.com/images/I/41KNN0N17BL.jpg",
                "link": "https://consumernotebook.com/nesco-fd-75pr-700-watt-food-dehydrator/4f3c0164ebae26000400003b/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f3c0164ebae26000400003b/",
                "title": "Nesco FD-75PR 700-Watt Food Dehydrator"
            },
            {
                "comment": "Good for not filling up your oven with something that takes hours to cook. Also allows you to carry your kitchen efforts to other locations.",
                "external_link": "http://www.amazon.com/gp/product/B001E5CWVU/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f3c0169ebae260004000086",
                "image_url": "http://ecx.images-amazon.com/images/I/41OtZjbJHsL.jpg",
                "link": "https://consumernotebook.com/cuisinart-psc-350-3-12-quart-programmable-slow-cooker/4f3c0169ebae260004000086/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f3c0169ebae260004000086/",
                "title": "Cuisinart PSC-350 3-1/2-Quart Programmable Slow Cooker"
            },
            {
                "comment": "Giant corn popper thingee!",
                "external_link": "http://www.amazon.com/gp/product/B002JM100Q/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f3c016aebae260004000099",
                "image_url": "http://ecx.images-amazon.com/images/I/41ZqYL-RUCL.jpg",
                "link": "https://consumernotebook.com/west-bend-82386-kettle-krazy-popcorn-popper-and-nut-roaster/4f3c016aebae260004000099/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f3c016aebae260004000099/",
                "title": "West Bend 82386 Kettle Krazy Popcorn Popper and Nut Roaster"
            },
            {
                "comment": "This seems like an awesome fruit dryer. Shelves! I think this is the one I want.",
                "external_link": "http://www.amazon.com/gp/product/B001P2J3K0/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f3c016aebae2600040000a3",
                "image_url": "http://ecx.images-amazon.com/images/I/41S5bKbppZL.jpg",
                "link": "https://consumernotebook.com/excalibur-3900-deluxe-series-9-tray-food-dehydrator-black/4f3c016aebae2600040000a3/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f3c016aebae2600040000a3/",
                "title": "Excalibur 3900 Deluxe Series 9 Tray Food Dehydrator - Black"
            },
            {
                "comment": "Great for any event! Large so the lazy susan property of this device is a a necessity.",
                "external_link": "http://www.amazon.com/gp/product/B005D6FWCC/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
                "id": "4f3c01afebae260004000282",
                "image_url": "http://ecx.images-amazon.com/images/I/41w8FbzTGuL.jpg",
                "link": "https://consumernotebook.com/crock-pot-scrtd305-bs-1-quart-triple-dipper-food-warmer-stainless-steel/4f3c01afebae260004000282/",
                "price_range": "Coming",
                "resource_uri": "/api/v1/products/4f3c01afebae260004000282/",
                "title": "Crock-Pot SCRTD305-BS 1-Quart Triple Dipper Food Warmer, Stainless Steel"
            }],
            "resource_uri": "/api/v1/lists/pydanny/fun-home-appliances/",
            "slug": "fun-home-appliances",
            "title": "Fun Home Appliances",
            "url": "http://consumernotebook.com/lists/pydanny/fun-home-appliances/"
        }]
    }