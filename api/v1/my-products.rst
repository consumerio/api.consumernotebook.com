.. _api-v1-my-products:

========================
GET /api/v1/my-products/
========================

Returns products you've interacted with in some way. You may not have added them to the system,
but you've added them to lists, grids, or just bookmarked them.

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

    curl https://consumernotebook.com/api/v1/my-products/ -d access_token={access_token} -G
    
Results:    

.. sourcecode:: javascript

    {
        "meta": {
            "limit": 20,
            "next": "/api/v1/my-products/?access_token={access_token}&limit=20&offset=20",
            "offset": 0,
            "previous": null,
            "total_count": 306
        },
        "objects": [{
            "creator": "pydanny",
            "grids": [],
            "id": "4f695015a08288000c000000",
            "image_url": "http://ecx.images-amazon.com/images/I/51XkcBwBe5L.jpg",
            "lists": [{
                "description": "",
                "id": 532,
                "resource_uri": "/api/v1/lists/532/",
                "title": "Kinect Games"
            }],
            "price_range": "$50-100",
            "resource_uri": "/api/v1/my-products/4f695015a08288000c000000/",
            "title": "Wipeout In the Zone: Xbox 360",
            "url": "http://www.amazon.com/gp/product/B004T7PWZ8/?ie=UTF8&tag=cn-001-20&linkCode=ur2"
        },
        {
            "creator": "pydanny",
            "grids": [],
            "id": "4f68b6dc74f2a0000e000019",
            "image_url": "http://ecx.images-amazon.com/images/I/51Mwj2UfegL.jpg",
            "lists": [{
                "description": "",
                "id": 532,
                "resource_uri": "/api/v1/lists/532/",
                "title": "Kinect Games"
            }],
            "price_range": "$10-20",
            "resource_uri": "/api/v1/my-products/4f68b6dc74f2a0000e000019/",
            "title": "Kinect Joy Ride: Video Games",
            "url": "http://www.amazon.com/gp/product/B002I0JC72/?ie=UTF8&tag=cn-001-20&linkCode=ur2"
        },
        {
            "creator": "pydanny",
            "grids": [],
            "id": "4f68b69e74f2a0000c00000d",
            "image_url": "http://ecx.images-amazon.com/images/I/51qAozec0aL.jpg",
            "lists": [{
                "description": "",
                "id": 532,
                "resource_uri": "/api/v1/lists/532/",
                "title": "Kinect Games"
            }],
            "price_range": "$20-50",
            "resource_uri": "/api/v1/my-products/4f68b69e74f2a0000c00000d/",
            "title": "Kinect Sports Season Two: Video Games",
            "url": "http://www.amazon.com/gp/product/B0050SYZ2G/?ie=UTF8&tag=cn-001-20&linkCode=ur2"
        },
        {
            "creator": "pydanny",
            "grids": [],
            "id": "4f68b66c74f2a0000d00000e",
            "image_url": "http://ecx.images-amazon.com/images/I/51iWCk9RSAL.jpg",
            "lists": [{
                "description": "",
                "id": 532,
                "resource_uri": "/api/v1/lists/532/",
                "title": "Kinect Games"
            },
            {
                "description": "This is a list of odds and ends I would like to get into my hands. Or at least my Kindle!",
                "id": 5,
                "resource_uri": "/api/v1/lists/5/",
                "title": "My Wishlist"
            }],
            "price_range": "$50-100",
            "resource_uri": "/api/v1/my-products/4f68b66c74f2a0000d00000e/",
            "title": "Forza Motorsport 4: Xbox 360",
            "url": "http://www.amazon.com/gp/product/B003O6E986/?ie=UTF8&tag=cn-001-20&linkCode=ur2"
        },
        {
            "creator": "pydanny",
            "grids": [],
            "id": "4f68b62174f2a0000c00000b",
            "image_url": "http://ecx.images-amazon.com/images/I/51oNpZEXJ6L.jpg",
            "lists": [{
                "description": "",
                "id": 532,
                "resource_uri": "/api/v1/lists/532/",
                "title": "Kinect Games"
            }],
            "price_range": "$50-100",
            "resource_uri": "/api/v1/my-products/4f68b62174f2a0000c00000b/",
            "title": "Kinect Star Wars: Video Games",
            "url": "http://www.amazon.com/gp/product/B002I0HCNI/?ie=UTF8&tag=cn-001-20&linkCode=ur2"
        },
        {
            "creator": "pydanny",
            "grids": [],
            "id": "4f68b5ef74f2a0000e000017",
            "image_url": "http://ecx.images-amazon.com/images/I/517WrLQT7iL.jpg",
            "lists": [{
                "description": "",
                "id": 532,
                "resource_uri": "/api/v1/lists/532/",
                "title": "Kinect Games"
            }],
            "price_range": "$50-100",
            "resource_uri": "/api/v1/my-products/4f68b5ef74f2a0000e000017/",
            "title": "Mass Effect 3: Xbox 360: Video Games",
            "url": "http://www.amazon.com/gp/product/B004FYEZMQ/?ie=UTF8&tag=cn-001-20&linkCode=ur2"
        },
        {
            "creator": "pydanny",
            "grids": [],
            "id": "4f68b47e74f2a0000e000015",
            "image_url": "http://ecx.images-amazon.com/images/I/61HutgxL-jL.jpg",
            "lists": [{
                "description": "This is a list of odds and ends I would like to get into my hands. Or at least my Kindle!",
                "id": 5,
                "resource_uri": "/api/v1/lists/5/",
                "title": "My Wishlist"
            }],
            "price_range": "$20-50",
            "resource_uri": "/api/v1/my-products/4f68b47e74f2a0000e000015/",
            "title": "SSX: Xbox 360",
            "url": "http://www.amazon.com/gp/product/B003O6C9LK/?ie=UTF8&tag=cn-001-20&linkCode=ur2"
        },
        {
            "creator": "pydanny",
            "grids": [],
            "id": "4f657b759007d7000e000002",
            "image_url": "http://ecx.images-amazon.com/images/I/51CuKsKGF8L.jpg",
            "lists": [{
                "description": "Here is a straight-forward list of books I want to read.",
                "id": 396,
                "resource_uri": "/api/v1/lists/396/",
                "title": "Book wishlist"
            },
            {
                "description": "This is a list of odds and ends I would like to get into my hands. Or at least my Kindle!",
                "id": 5,
                "resource_uri": "/api/v1/lists/5/",
                "title": "My Wishlist"
            }],
            "price_range": "$0-10",
            "resource_uri": "/api/v1/my-products/4f657b759007d7000e000002/",
            "title": "Questions for a Soldier eBook: John Scalzi",
            "url": "http://www.amazon.com/gp/product/B005OTEEEA/?ie=UTF8&tag=cn-001-20&linkCode=ur2"
        },
        {
            "creator": "pydanny",
            "grids": [],
            "id": "4f650c89931314000d000000",
            "image_url": "http://ecx.images-amazon.com/images/I/51vvGdFBs1L.jpg",
            "lists": [{
                "description": "Here is a straight-forward list of books I want to read.",
                "id": 396,
                "resource_uri": "/api/v1/lists/396/",
                "title": "Book wishlist"
            },
            {
                "description": "This is a list of odds and ends I would like to get into my hands. Or at least my Kindle!",
                "id": 5,
                "resource_uri": "/api/v1/lists/5/",
                "title": "My Wishlist"
            }],
            "price_range": "$0-10",
            "resource_uri": "/api/v1/my-products/4f650c89931314000d000000/",
            "title": "The Sagan Diary eBook: John Scalzi: Kindle Store",
            "url": "http://www.amazon.com/gp/product/B005OTDQQ2/?ie=UTF8&tag=cn-001-20&linkCode=ur2"
        },
        {
            "creator": "pydanny",
            "grids": [{
                "description": "",
                "id": "4f615025e0eac7000c00000c",
                "resource_uri": "/api/v1/grids/4f615025e0eac7000c00000c/",
                "title": "Super Cheap Cell Phones"
            }],
            "id": "4f6150d5e0eac7000d000010",
            "image_url": "http://images10.newegg.com/NeweggImage/ProductImageCompressAll300/75-176-114-03.jpg",
            "lists": [],
            "price_range": "$50-100",
            "resource_uri": "/api/v1/my-products/4f6150d5e0eac7000d000010/",
            "title": "Newegg.com - SAMSUNG BlackJack II Black 3G Unlocked Cell w/ Windows Mobile OS / GPS / Full QWERTY Ke",
            "url": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.newegg.com/Product/Product.aspx%3FItem%3DN82E16875176114"
        },
        {
            "creator": "pydanny",
            "grids": [{
                "description": "",
                "id": "4f615025e0eac7000c00000c",
                "resource_uri": "/api/v1/grids/4f615025e0eac7000c00000c/",
                "title": "Super Cheap Cell Phones"
            }],
            "id": "4f615051e0eac7000e000009",
            "image_url": "http://images17.newegg.com/is/image/newegg/75-704-012-TS?$S300W$",
            "lists": [],
            "price_range": "$50-100",
            "resource_uri": "/api/v1/my-products/4f615051e0eac7000e000009/",
            "title": "Newegg.com - Unnecto SHELL Silver Unlocked Cell Phone w/ Dual Sim",
            "url": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.newegg.com/Product/Product.aspx%3FItem%3DN82E16875704012"
        },
        {
            "creator": "pydanny",
            "grids": [{
                "description": "",
                "id": "4f615025e0eac7000c00000c",
                "resource_uri": "/api/v1/grids/4f615025e0eac7000c00000c/",
                "title": "Super Cheap Cell Phones"
            }],
            "id": "4f615025e0eac7000c00000b",
            "image_url": "http://images17.newegg.com/is/image/newegg/75-104-018-TS?$S300W$",
            "lists": [],
            "price_range": "$20-50",
            "resource_uri": "/api/v1/my-products/4f615025e0eac7000c00000b/",
            "title": "Newegg.com - SHARP Sidekick LX 2009 Orchid Unlocked GSM Smart Phone w/ Full QWERTY Keyboard",
            "url": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.newegg.com/Product/Product.aspx%3FItem%3DN82E16875104018"
        },
        {
            "creator": "pydanny",
            "grids": [],
            "id": "4f60423ae0eac7000c000004",
            "image_url": "http://ecx.images-amazon.com/images/I/317mnvx8axL.jpg",
            "lists": [{
                "description": "This is a list of odds and ends I would like to get into my hands. Or at least my Kindle!",
                "id": 5,
                "resource_uri": "/api/v1/lists/5/",
                "title": "My Wishlist"
            }],
            "price_range": "$50-100",
            "resource_uri": "/api/v1/my-products/4f60423ae0eac7000c000004/",
            "title": "Vibram Fivefingers Komodosport Ls Mens Running Shoes",
            "url": "http://www.amazon.com/gp/product/B005CQRTOW/?ie=UTF8&tag=cn-001-20&linkCode=ur2"
        },
        {
            "creator": "pydanny",
            "grids": [{
                "description": "These are books I've really enjoying having in my career as a professional Python developer.",
                "id": "4f319564bf8bbd000a000000",
                "resource_uri": "/api/v1/grids/4f319564bf8bbd000a000000/",
                "title": "Must-Have Python Programming Books "
            }],
            "id": "4f5bd9381cfd5d000c00000a",
            "image_url": "http://ecx.images-amazon.com/images/I/51qvS8cyLCL.jpg",
            "lists": [{
                "description": "This is a list of every Python programming book I can find. Let me know if you find one not on this list!",
                "id": 36,
                "resource_uri": "/api/v1/lists/36/",
                "title": "Complete List of Python Programming Books"
            }],
            "price_range": "$20-50",
            "resource_uri": "/api/v1/my-products/4f5bd9381cfd5d000c00000a/",
            "title": "Core Python Programming (2nd Edition) by Wesley J Chun",
            "url": "http://www.amazon.com/gp/product/0132269937/?ie=UTF8&tag=cn-001-20&linkCode=ur2"
        },
        {
            "creator": "pydanny",
            "grids": [],
            "id": "4f5bc32f24b4b3000d000005",
            "image_url": "http://ecx.images-amazon.com/images/I/41S40M67EdL._SL500_AA300_.jpg",
            "lists": [],
            "price_range": "$50-100",
            "resource_uri": "/api/v1/my-products/4f5bc32f24b4b3000d000005/",
            "title": "Cantilever LCD Monitor TV Arm Bracket Wall Mount with: Amazon.co.uk: Electronics",
            "url": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.amazon.co.uk/Cantilever-Monitor-Bracket-Mount-Swivel/dp/B002JCBU7Y/ref%3Dpd_cp_ce_1"
        },
        {
            "creator": "pydanny",
            "grids": [{
                "description": "",
                "id": "4f5bb18b1cfd5d000e000003",
                "resource_uri": "/api/v1/grids/4f5bb18b1cfd5d000e000003/",
                "title": "camping lanterns"
            }],
            "id": "4f5bb97024b4b3000c000001",
            "image_url": "http://ecx.images-amazon.com/images/I/41W1xVOr69L._SL500_AA300_.jpg",
            "lists": [{
                "description": "This is a list of odds and ends I would like to get into my hands. Or at least my Kindle!",
                "id": 5,
                "resource_uri": "/api/v1/lists/5/",
                "title": "My Wishlist"
            }],
            "price_range": "$100-200",
            "resource_uri": "/api/v1/my-products/4f5bb97024b4b3000c000001/",
            "title": "Fujifilm FinePix L55 Digital Camera - Black 2.4 inch",
            "url": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//www.amazon.co.uk/gp/product/B005NZJPCG/ref%3Ds9_ri_gw_g23_ir03%3Fpf_rd_m%3DA3P5ROKL5A1OLE%26pf_rd_s%3Dcenter-3%26pf_rd_r%3D0E04WE11GEQPYQCY60KR%26pf_rd_t%3D101%26pf_rd_p%3D202006527%26pf_rd_i%3D468294"
        },
        {
            "creator": "pydanny",
            "grids": [{
                "description": "",
                "id": "4f5bb18b1cfd5d000e000003",
                "resource_uri": "/api/v1/grids/4f5bb18b1cfd5d000e000003/",
                "title": "camping lanterns"
            }],
            "id": "4f5bb63b36a633000e000008",
            "image_url": "http://ecx.images-amazon.com/images/I/41PGb7VsQBL.jpg",
            "lists": [],
            "price_range": "$20-50",
            "resource_uri": "/api/v1/my-products/4f5bb63b36a633000e000008/",
            "title": "Rayovac SE3DLN Sportsman Xtreme 300-Lumen LED Lantern: Home Improvement",
            "url": "http://www.amazon.com/gp/product/B0018S4XIS/?ie=UTF8&tag=cn-001-20&linkCode=ur2"
        },
        {
            "creator": "pydanny",
            "grids": [{
                "description": "",
                "id": "4f5bb18b1cfd5d000e000003",
                "resource_uri": "/api/v1/grids/4f5bb18b1cfd5d000e000003/",
                "title": "camping lanterns"
            }],
            "id": "4f5bb18b1cfd5d000e000002",
            "image_url": "http://ecx.images-amazon.com/images/I/41hUO1aAHbL.jpg",
            "lists": [{
                "description": "This is a list of odds and ends I would like to get into my hands. Or at least my Kindle!",
                "id": 5,
                "resource_uri": "/api/v1/lists/5/",
                "title": "My Wishlist"
            }],
            "price_range": "$50-100",
            "resource_uri": "/api/v1/my-products/4f5bb18b1cfd5d000e000002/",
            "title": "Coleman LED Quad Lantern: Sports & Outdoors",
            "url": "http://www.amazon.com/gp/product/B001TS71NG/?ie=UTF8&tag=cn-001-20&linkCode=ur2"
        },
        {
            "creator": "pydanny",
            "grids": [],
            "id": "4f5bae6a1cfd5d000d00000a",
            "image_url": null,
            "lists": [{
                "description": "This is a list of odds and ends I would like to get into my hands. Or at least my Kindle!",
                "id": 5,
                "resource_uri": "/api/v1/lists/5/",
                "title": "My Wishlist"
            }],
            "price_range": "$50-100",
            "resource_uri": "/api/v1/my-products/4f5bae6a1cfd5d000d00000a/",
            "title": "Eton Self-Powered Safety Hub with Weather Radio and USB Cell Phone Charger",
            "url": "http://www.amazon.com/gp/product/B005A40HJK/?ie=UTF8&tag=cn-001-20&linkCode=ur2"
        },
        {
            "creator": "pydanny",
            "grids": [],
            "id": "4f5bab081cfd5d000c000008",
            "image_url": "http://ecx.images-amazon.com/images/I/51gcyDU9V%2BL.jpg",
            "lists": [],
            "price_range": "$50-100",
            "resource_uri": "/api/v1/my-products/4f5bab081cfd5d000c000008/",
            "title": "Your Shape Fitness Evolved: Video Games",
            "url": "http://www.amazon.com/gp/product/B002I0H9WM/?ie=UTF8&tag=cn-001-20&linkCode=ur2"
        }]
    }