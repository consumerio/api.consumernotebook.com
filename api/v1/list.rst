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

    curl https://consumernotebook.com/api/v1/lists/pydanny/complete-list-of-python-programming-books/ -d access_token={access_token} -G
    
Results:    

.. sourcecode:: javascript

    {
        "created": "2011-12-05T09:37:10.328231",
        "description": "This is a list of every Python programming book I can find. Let me know if you find one not on this list!",
        "id": "36",
        "last_modified_by_user": "2012-03-09T14:26:58.210396",
        "modified": "2012-03-17T21:32:31.404607",
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
            "comment": "Numpy is awesome! I want to use it more.",
            "id": "4f3c0163ebae26000400002d",
            "image_url": "http://ecx.images-amazon.com/images/I/51o0XqA%2BsLL.jpg",
            "price_range": "Coming",
            "resource_url": "/api/v1/products/4f3c0163ebae26000400002d/",
            "title": "NumPy 1.5 Beginner's Guide"
        },
        {
            "external_link": "http://www.amazon.com/gp/product/1430210478/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
            "comment": "",
            "id": "4f3c0164ebae260004000043",
            "image_url": "http://ecx.images-amazon.com/images/I/41Ry%2BLUNkQL.jpg",
            "price_range": "$20-50",
            "resource_url": "/api/v1/products/4f3c0164ebae260004000043/",
            "title": "Pro Django (Expert's Voice in Web Development)"
        },
        {
            "external_link": "http://www.amazon.com/gp/product/143021936X/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
            "comment": "",
            "id": "4f3c0168ebae260004000070",
            "image_url": "http://ecx.images-amazon.com/images/I/5198kKFjb2L.jpg",
            "price_range": "$20-50",
            "resource_url": "/api/v1/products/4f3c0168ebae260004000070/",
            "title": "The Definitive Guide to Django: Web Development Done Right"
        },
        {
            "external_link": "http://www.amazon.com/gp/product/0321767349/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
            "comment": "Released in early 2011, this is an enormous book but worth the weight. Think of it as combining the cookbook and essential reference and you've got an idea as to what this book gives you. This book is unbelievable in it's depth and quality.",
            "id": "4f3c016bebae2600040000bc",
            "image_url": "http://ecx.images-amazon.com/images/I/518kgosz6XL.jpg",
            "price_range": "$20-50",
            "resource_url": "/api/v1/products/4f3c016bebae2600040000bc/",
            "title": "The Python Standard Library by Example (Developer's Library)"
        },
        {
            "external_link": "http://www.amazon.com/gp/product/0672329786/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
            "comment": "This is/was a great book for programming in Python. It is a library by library reference for programming in Python. In quiet moments I used to slow peruse the pages to make sure I knew all the great bits that Python gave me out of the box. It is a bit dated now, but still quite useful.",
            "id": "4f3c0176ebae2600040000d8",
            "image_url": "http://ecx.images-amazon.com/images/I/41m7YwHS18L.jpg",
            "price_range": "$20-50",
            "resource_url": "/api/v1/products/4f3c0176ebae2600040000d8/",
            "title": "Python Essential Reference (4th Edition)"
        },
        {
            "external_link": "http://www.amazon.com/gp/product/0596158068/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
            "comment": "In 2005 I learned Python from the 2003 edition of this book. Most of it was great and quite useful, except for the three chapters on Jython. Other people swear by Dive into Python but I found this a much clearer way to get into the language. These days I recommend Zed Shaw's Learn Python the Hard Way, but this is still a good resource for beginning Python developers.",
            "id": "4f3c0177ebae2600040000f1",
            "image_url": "http://ecx.images-amazon.com/images/I/51LHOKdyWML.jpg",
            "price_range": "$20-50",
            "resource_url": "/api/v1/products/4f3c0177ebae2600040000f1/",
            "title": "Learning Python: Powerful Object-Oriented Programming"
        },
        {
            "external_link": "http://www.amazon.com/gp/product/0132356139/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
            "comment": "",
            "id": "4f3c0188ebae26000400014e",
            "image_url": "http://ecx.images-amazon.com/images/I/41c1QK1THKL.jpg",
            "price_range": "$20-50",
            "resource_url": "/api/v1/products/4f3c0188ebae26000400014e/",
            "title": "Python Web Development with Django"
        },
        {
            "external_link": "http://www.amazon.com/gp/product/B006OYO9SK/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
            "comment": "",
            "id": "4f3c018aebae26000400015c",
            "image_url": "http://ecx.images-amazon.com/images/I/312kliN4qdL.jpg",
            "price_range": "$20-50",
            "resource_url": "/api/v1/products/4f3c018aebae26000400015c/",
            "title": "Django Design Patterns"
        },
        {
            "external_link": "http://www.amazon.com/gp/product/0596158084/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
            "comment": "I have this weird thing about good pocket references - I find them as useful for learning things about tools as I do the monstrous tomes. This qualifies as one of those super useful references that justifies a purchase. You can't go wrong with this, especially considering the price. Great for picking up core Python built-ins as well as all the the awesome methods on the native types.",
            "id": "4f3c019eebae2600040001bc",
            "image_url": "http://ecx.images-amazon.com/images/I/51UsBNYpCtL.jpg",
            "price_range": "$10-20",
            "resource_url": "/api/v1/products/4f3c019eebae2600040001bc/",
            "title": "Python Pocket Reference"
        },
        {
            "external_link": "http://www.amazon.com/gp/product/1847197566/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
            "comment": "",
            "id": "4f3c019febae2600040001d0",
            "image_url": "http://ecx.images-amazon.com/images/I/41A0xBtW5PL.jpg",
            "price_range": "$20-50",
            "resource_url": "/api/v1/products/4f3c019febae2600040001d0/",
            "title": "Django 1.1 Testing and Debugging"
        },
        {
            "external_link": "http://www.amazon.com/gp/product/0596007973/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
            "comment": "Being a series of recipes for solving various problems in Python, this is an amazing, wonderful book. In 2006 for the holidays I landed two copies as presents, and the book is so good I kept them both. One for the office and one for home! This is a great reference and full of wonderful gems and tricks for Python developers of all types.",
            "id": "4f3c01a7ebae260004000235",
            "image_url": "http://ecx.images-amazon.com/images/I/51LY8uDISuL.jpg",
            "price_range": "$20-50",
            "resource_url": "/api/v1/products/4f3c01a7ebae260004000235/",
            "title": "Python Cookbook"
        },
        {
            "external_link": "http://www.amazon.com/gp/product/1847196780/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
            "comment": "",
            "id": "4f3c01aaebae260004000258",
            "image_url": "http://ecx.images-amazon.com/images/I/511QYiLPJbL.jpg",
            "price_range": "$20-50",
            "resource_url": "/api/v1/products/4f3c01aaebae260004000258/",
            "title": "Django 1.0 Website Development"
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
            "external_link": "http://www.amazon.com/gp/product/125785321X/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
            "comment": "",
            "id": "4f45bd9586f5df000e000000",
            "image_url": "http://ecx.images-amazon.com/images/I/51gLdcig8QL.jpg",
            "price_range": "Coming",
            "resource_url": "/api/v1/products/4f45bd9586f5df000e000000/",
            "title": "Learn Python the Hard Way (9781257853212): Zed Shaw: Books"
        },
        {
            "external_link": "http://go.consumernotebook.com?id=26908X855841&xs=1&url=http%3A//shop.oreilly.com/product/9780596515829.do",
            "comment": "",
            "id": "4f45f7c7e114f002ae000000",
            "image_url": "http://akamaicovers.oreilly.com/images/9780596515829/cat.gif",
            "price_range": "Coming",
            "resource_url": "/api/v1/products/4f45f7c7e114f002ae000000/",
            "title": "Python for Unix and Linux System Administration"
        },
        {
            "external_link": "http://www.amazon.com/gp/product/1449382673/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
            "comment": "",
            "id": "4f45f817e114f00364000000",
            "image_url": "http://ecx.images-amazon.com/images/I/51I1iu7LvQL.jpg",
            "price_range": "Coming",
            "resource_url": "/api/v1/products/4f45f817e114f00364000000/",
            "title": "Head First Python by Paul Barry"
        },
        {
            "external_link": "http://www.amazon.com/gp/product/1430227575/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
            "comment": "",
            "id": "4f45f888e114f002ae000002",
            "image_url": "http://ecx.images-amazon.com/images/I/51hPupkbaQL.jpg",
            "price_range": "Coming",
            "resource_url": "/api/v1/products/4f45f888e114f002ae000002/",
            "title": "Pro Python: Marty Alchin"
        },
        {
            "external_link": "http://www.amazon.com/gp/product/184719494X/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
            "comment": "",
            "id": "4f45f8ea914b6302ac000000",
            "image_url": "http://ecx.images-amazon.com/images/I/51yEgqyNZvL.jpg",
            "price_range": "Coming",
            "resource_url": "/api/v1/products/4f45f8ea914b6302ac000000/",
            "title": "Expert Python Programming by Tarek Ziad\u00e9"
        },
        {
            "external_link": "http://www.amazon.com/gp/product/1590599810/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
            "comment": "",
            "id": "4f45f917914b630326000000",
            "image_url": "http://ecx.images-amazon.com/images/I/514nuZLtMHL.jpg",
            "price_range": "Coming",
            "resource_url": "/api/v1/products/4f45f917914b630326000000/",
            "title": "Foundations of Agile Python Development: Jeff Younker"
        },
        {
            "external_link": "http://www.amazon.com/gp/product/1847198848/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
            "comment": "",
            "id": "4f45f941914b630326000002",
            "image_url": "http://ecx.images-amazon.com/images/I/41izoWan1zL.jpg",
            "price_range": "Coming",
            "resource_url": "/api/v1/products/4f45f941914b630326000002/",
            "title": "Python Testing: Beginner's Guide by Daniel Arbuckle"
        },
        {
            "external_link": "http://www.amazon.com/gp/product/1430232374/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
            "comment": "",
            "id": "4f45f98238093902b3000000",
            "image_url": "http://ecx.images-amazon.com/images/I/51xcs3V09xL.jpg",
            "price_range": "Coming",
            "resource_url": "/api/v1/products/4f45f98238093902b3000000/",
            "title": "Python Algorithms: Mastering Basic Algorithms in the Python Language by Magnus Lie Hetland"
        },
        {
            "external_link": "http://www.amazon.com/gp/product/1849511268/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
            "comment": "",
            "id": "4f45f9a0914b6302ad000000",
            "image_url": "http://ecx.images-amazon.com/images/I/51f7HTYaEbL.jpg",
            "price_range": "Coming",
            "resource_url": "/api/v1/products/4f45f9a0914b6302ad000000/",
            "title": "Python 3 Object Oriented Programming by Dusty Phillips"
        },
        {
            "external_link": "http://www.amazon.com/gp/product/1430216328/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
            "comment": "",
            "id": "4f45f9c0e114f00364000004",
            "image_url": "http://ecx.images-amazon.com/images/I/5108IBveuUL.jpg",
            "price_range": "Coming",
            "resource_url": "/api/v1/products/4f45f9c0e114f00364000004/",
            "title": "Python 3 for Absolute Beginners by Tim Hall and J-P Stacey"
        },
        {
            "external_link": "http://www.amazon.com/gp/product/1430226056/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
            "comment": "",
            "id": "4f45f9dd914b6302ac000004",
            "image_url": "http://ecx.images-amazon.com/images/I/41AFCYqRt%2BL.jpg",
            "price_range": "Coming",
            "resource_url": "/api/v1/products/4f45f9dd914b6302ac000004/",
            "title": "Pro Python System Administration by  Rytis Sileika"
        },
        {
            "external_link": "http://www.amazon.com/gp/product/0596100469/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
            "comment": "",
            "id": "4f45f9f2914b6302ad000004",
            "image_url": "http://ecx.images-amazon.com/images/I/51ChOtzK6ML.jpg",
            "price_range": "Coming",
            "resource_url": "/api/v1/products/4f45f9f2914b6302ad000004/",
            "title": "Python in a Nutshell, Second Edition by Alex Martelli"
        },
        {
            "external_link": "http://www.amazon.com/gp/product/1590598725/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
            "comment": "",
            "id": "4f45fa0938093902b2000000",
            "image_url": "http://ecx.images-amazon.com/images/I/51XWVW%2BWBEL.jpg",
            "price_range": "Coming",
            "resource_url": "/api/v1/products/4f45fa0938093902b2000000/",
            "title": "Beginning Game Development with Python and Pygame: From Novice to Professional by Will McGugan"
        },
        {
            "external_link": "http://www.amazon.com/gp/product/1935182080/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
            "comment": "",
            "id": "4f45fa6d914b6302ac000008",
            "image_url": "http://ecx.images-amazon.com/images/I/41eyXaqJexL.jpg",
            "price_range": "Coming",
            "resource_url": "/api/v1/products/4f45fa6d914b6302ac000008/",
            "title": "Hello! Python by Anthony S. Briggs"
        },
        {
            "external_link": "http://www.amazon.com/gp/product/0982106017/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
            "comment": "",
            "id": "4f45fac1914b6302ac00000a",
            "image_url": "http://ecx.images-amazon.com/images/I/51uOL93WYBL.jpg",
            "price_range": "Coming",
            "resource_url": "/api/v1/products/4f45fac1914b6302ac00000a/",
            "title": "Invent Your Own Computer Games with Python, 2nd Edition by Al Sweigart"
        },
        {
            "external_link": "http://www.amazon.com/gp/product/1435460979/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
            "comment": "",
            "id": "4f45fad6e114f002ae000004",
            "image_url": "http://ecx.images-amazon.com/images/I/51MVF-mD5xL.jpg",
            "price_range": "Coming",
            "resource_url": "/api/v1/products/4f45fad6e114f002ae000004/",
            "title": "Introduction to Python Programming and Developing GUI Applications with PyQT by B. M. Harwani"
        },
        {
            "external_link": "http://www.amazon.com/gp/product/193518220X/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
            "comment": "",
            "id": "4f45faef38093902b2000002",
            "image_url": "http://ecx.images-amazon.com/images/I/41RhhdfdTwL.jpg",
            "price_range": "Coming",
            "resource_url": "/api/v1/products/4f45faef38093902b2000002/",
            "title": "The Quick Python Book, Second Edition by Vern Ceder"
        },
        {
            "external_link": "http://www.amazon.com/gp/product/1849965366/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
            "comment": "",
            "id": "4f45fb0c3809390274000002",
            "image_url": "http://ecx.images-amazon.com/images/I/41Cje6UvUOL.jpg",
            "price_range": "Coming",
            "resource_url": "/api/v1/products/4f45fb0c3809390274000002/",
            "title": "Python Programming Fundamentals by Kent D. Lee"
        },
        {
            "external_link": "http://www.amazon.com/gp/product/1590282418/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
            "comment": "",
            "id": "4f45fb293809390274000004",
            "image_url": "http://ecx.images-amazon.com/images/I/51ySXyRK5qL.jpg",
            "price_range": "Coming",
            "resource_url": "/api/v1/products/4f45fb293809390274000004/",
            "title": "Python Programming: An Introduction to Computer Science 2nd Edition by John Zelle"
        },
        {
            "external_link": "http://www.amazon.com/gp/product/1933988495/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
            "comment": "",
            "id": "4f45fb44e114f002ae000006",
            "image_url": "http://ecx.images-amazon.com/images/I/51PT1ve6nLL.jpg",
            "price_range": "Coming",
            "resource_url": "/api/v1/products/4f45fb44e114f002ae000006/",
            "title": "Hello World! Computer Programming for Kids and Other Beginners by Warren Sande, Carter Sande"
        },
        {
            "external_link": "http://www.amazon.com/gp/product/0321680561/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
            "comment": "",
            "id": "4f4603dae72fcf0102000000",
            "image_url": "http://ecx.images-amazon.com/images/I/51OfHZsM5zL.jpg",
            "price_range": "Coming",
            "resource_url": "/api/v1/products/4f4603dae72fcf0102000000/",
            "title": "Programming in Python 3: A Complete Introduction to the Python Language by Mark Summerfield"
        },
        {
            "external_link": "http://www.amazon.com/gp/product/0321112547/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
            "comment": "",
            "id": "4f460847103e2500c3000000",
            "image_url": "http://ecx.images-amazon.com/images/I/31td2Ii2kjL.jpg",
            "price_range": "Coming",
            "resource_url": "/api/v1/products/4f460847103e2500c3000000/",
            "title": "Text Processing in Python by David Mertz"
        },
        {
            "external_link": "http://www.amazon.com/gp/product/1933988339/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
            "comment": "",
            "id": "4f4692f8ffd8be054e000000",
            "image_url": "http://ecx.images-amazon.com/images/I/51cjWFbW5pL.jpg",
            "price_range": "Coming",
            "resource_url": "/api/v1/products/4f4692f8ffd8be054e000000/",
            "title": "IronPython in Action by Michael J. Foord, Christian Muirhead"
        },
        {
            "external_link": "http://www.amazon.com/gp/product/1430219629/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
            "comment": "",
            "id": "4f46932536593b0364000000",
            "image_url": "http://ecx.images-amazon.com/images/I/5159PI1DbdL.jpg",
            "price_range": "Coming",
            "resource_url": "/api/v1/products/4f46932536593b0364000000/",
            "title": "Pro IronPython by Alan Harris"
        },
        {
            "external_link": "http://www.amazon.com/gp/product/0470548592/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
            "comment": "",
            "id": "4f469330ffd8be054e000002",
            "image_url": "http://ecx.images-amazon.com/images/I/51rFmLdPeyL.jpg",
            "price_range": "Coming",
            "resource_url": "/api/v1/products/4f469330ffd8be054e000002/",
            "title": "Professional IronPython by John Paul Mueller"
        },
        {
            "external_link": "http://www.amazon.com/gp/product/1932394621/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
            "comment": "",
            "id": "4f4695021fad1d000e000000",
            "image_url": "http://ecx.images-amazon.com/images/I/41AEDpqzGSL.jpg",
            "price_range": "Coming",
            "resource_url": "/api/v1/products/4f4695021fad1d000e000000/",
            "title": "Wxpython in Action by Noel Rappin, Robin Dunn"
        },
        {
            "external_link": "http://www.amazon.com/gp/product/1849511780/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
            "comment": "",
            "id": "4f469511e87fee000c000000",
            "image_url": "http://ecx.images-amazon.com/images/I/519RmENFf1L.jpg",
            "price_range": "Coming",
            "resource_url": "/api/v1/products/4f469511e87fee000c000000/",
            "title": "wxPython 2.8 Application Development Cookbook by Cody Precord"
        },
        {
            "external_link": "http://www.amazon.com/gp/product/0596809565/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
            "comment": "",
            "id": "4f46952ee87fee000e000000",
            "image_url": "http://ecx.images-amazon.com/images/I/51q8JleClKL.jpg",
            "price_range": "Coming",
            "resource_url": "/api/v1/products/4f46952ee87fee000e000000/",
            "title": "Real World Instrumentation with Python by John M. Hughes"
        },
        {
            "external_link": "http://www.amazon.com/gp/product/B0057761SQ/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
            "comment": "",
            "id": "4f46955f1fad1d000e000002",
            "image_url": "http://ecx.images-amazon.com/images/I/5107sWosN-L.jpg",
            "price_range": "Coming",
            "resource_url": "/api/v1/products/4f46955f1fad1d000e000002/",
            "title": "wxPython 2.8 Application Development Cookbook eBook by Cody Precord"
        },
        {
            "external_link": "http://www.amazon.com/gp/product/1461182050/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
            "comment": "",
            "id": "4f469572e87fee000c000002",
            "image_url": "http://ecx.images-amazon.com/images/I/31fgjIfJ2GL.jpg",
            "price_range": "Coming",
            "resource_url": "/api/v1/products/4f469572e87fee000c000002/",
            "title": "Learning to Program Using Python by Cody Jackson"
        },
        {
            "external_link": "http://www.amazon.com/gp/product/B006ZHJSIM/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
            "comment": "",
            "id": "4f4695d5d6771d000d000000",
            "image_url": "http://ecx.images-amazon.com/images/I/51vQ-HXDsdL.jpg",
            "price_range": "Coming",
            "resource_url": "/api/v1/products/4f4695d5d6771d000d000000/",
            "title": "Guide to: Learning Python Decorators by Matt Harrison"
        },
        {
            "external_link": "http://www.amazon.com/gp/product/B00639H0AK/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
            "comment": "",
            "id": "4f4695e61fad1d000d000000",
            "image_url": "http://ecx.images-amazon.com/images/I/41RWay7GikL.jpg",
            "price_range": "Coming",
            "resource_url": "/api/v1/products/4f4695e61fad1d000d000000/",
            "title": "Treading on Python Volume 1 by Matt Harrison"
        },
        {
            "external_link": "http://www.amazon.com/gp/product/B005NHYZAQ/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
            "comment": "",
            "id": "4f469694e87fee000d000000",
            "image_url": "http://ecx.images-amazon.com/images/I/51gpNkQX3CL.jpg",
            "price_range": "Coming",
            "resource_url": "/api/v1/products/4f469694e87fee000d000000/",
            "title": "Python Geospatial Development by Erik Westra"
        },
        {
            "external_link": "http://www.amazon.com/gp/product/0132269937/?ie=UTF8&tag=cn-001-20&linkCode=ur2",
            "comment": "Wesley Chun is awesome",
            "id": "4f5bd9381cfd5d000c00000a",
            "image_url": "http://ecx.images-amazon.com/images/I/51qvS8cyLCL.jpg",
            "price_range": "$20-50",
            "resource_url": "/api/v1/products/4f5bd9381cfd5d000c00000a/",
            "title": "Core Python Programming (2nd Edition) by Wesley J Chun"
        }],
        "resource_uri": "/api/v1/lists/36/",
        "slug": "complete-list-of-python-programming-books",
        "title": "Complete List of Python Programming Books"
    }