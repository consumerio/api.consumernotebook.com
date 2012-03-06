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
            "next": "/api/v1/grids/?username=audreyr&apikey=72c9f72f2ea75b97c0d5b7117344c6a6&limit=20&offset=20",
            "offset": 0,
            "previous": null,
            "total_count": 41
        },
        "objects": [
        {
            "features": [{
                "description": "",
                "slug": "5c99096f-e24d-4e78-b443-37728fb65f57",
                "title": "Type"
            },
            {
                "description": "",
                "slug": "7c9e41ae-6454-4ffc-bf13-a6cb8694c968",
                "title": "Can browse the web"
            },
            {
                "description": "",
                "slug": "0c843de7-5446-4990-8315-b643b972807b",
                "title": "Streaming video sources supported"
            },
            {
                "description": "Use the web while watching live TV or other media.",
                "slug": "08cf2097-daa5-4139-a8f5-686a39419da1",
                "title": "Picture-in-picture"
            },
            {
                "description": "",
                "slug": "b895c004-2996-47a2-9128-be3e261a2221",
                "title": "Use phone as remote"
            },
            {
                "description": "I prefer remote controls with rubbery, tactile buttons. They're more ergonomic than touchscreens.",
                "slug": "c4fef42e-301e-4ad3-a921-d62eb65c49c4",
                "title": "Use a regular remote"
            },
            {
                "description": "",
                "slug": "045e8b26-3614-49b8-97a7-a5c6ca4f112f",
                "title": "Can download apps"
            },
            {
                "description": "",
                "slug": "94bec385-c665-49e9-b43c-c6a11fcf42c8",
                "title": "Connects to cable box, functions as DVR"
            },
            {
                "description": "",
                "slug": "1ee41dd2-eac0-4a92-8e3f-6038c4e5e42f",
                "title": "HD video calls"
            },
            {
                "description": "",
                "slug": "41b820c4-e7bb-4d40-aff5-124283c2e0d8",
                "title": "HD video support"
            },
            {
                "description": "",
                "slug": "bb86d008-57d7-4b0a-bb53-7a6544ebe88f",
                "title": "Ports/connections"
            }],
            "grid_items": 
                [
                    {
                        "created": "2012-02-29T12:38:01.644000",
                        "elements": {
                            "045e8b26-3614-49b8-97a7-a5c6ca4f112f": "[check] Android market apps for TV",
                            "08cf2097-daa5-4139-a8f5-686a39419da1": "[check]",
                            "0c843de7-5446-4990-8315-b643b972807b": "[p-3] Netflix, Amazon Instant Video, YouTube",
                            "1ee41dd2-eac0-4a92-8e3f-6038c4e5e42f": "[check] Requires separate $149 camera",
                            "41b820c4-e7bb-4d40-aff5-124283c2e0d8": "[p-5] Up to 1080p support",
                            "5c99096f-e24d-4e78-b443-37728fb65f57": "Google TV box",
                            "7c9e41ae-6454-4ffc-bf13-a6cb8694c968": "[check] Google Chrome",
                            "94bec385-c665-49e9-b43c-c6a11fcf42c8": "[check] DVR integration with DISH Network",
                            "b895c004-2996-47a2-9128-be3e261a2221": "[check] Android, iPhone, iPad, or iPod Touch",
                            "bb86d008-57d7-4b0a-bb53-7a6544ebe88f": "Ethernet, USB, HDMI, optical audio, 802.11 a/b/g/n Wi-Fi",
                            "c4fef42e-301e-4ad3-a921-d62eb65c49c4": "[p-3] A mini-remote is available for $129"
                        },
                        "id": "4f4e8ca9cac041000d000003"
                    },
                    {
                        "created": "2012-02-29T12:34:18.002000",
                        "elements": {
                            "045e8b26-3614-49b8-97a7-a5c6ca4f112f": "[check] Android market apps for TV",
                            "08cf2097-daa5-4139-a8f5-686a39419da1": "[check]",
                            "0c843de7-5446-4990-8315-b643b972807b": "[p-3] Netflix, Amazon Instant Video, YouTube",
                            "1ee41dd2-eac0-4a92-8e3f-6038c4e5e42f": "[x]",
                            "41b820c4-e7bb-4d40-aff5-124283c2e0d8": "[p-5] Up to 1080p support",
                            "5c99096f-e24d-4e78-b443-37728fb65f57": "Google TV box",
                            "7c9e41ae-6454-4ffc-bf13-a6cb8694c968": "[check] Google Chrome",
                            "94bec385-c665-49e9-b43c-c6a11fcf42c8": "[check] DVR integration with DISH Network",
                            "b895c004-2996-47a2-9128-be3e261a2221": "[check] Android, iPhone, iPad, or iPod Touch",
                            "bb86d008-57d7-4b0a-bb53-7a6544ebe88f": "Ethernet, USB, HDMI, optical audio, Wi-Fi",
                            "c4fef42e-301e-4ad3-a921-d62eb65c49c4": "[p-5] Comes with an amazing remote that's half video game controller, half QWERTY mini-keyboard"
                        },
                        "id": "4f4e8bc9cac041000c000000"
                    },
                    {
                        "created": "2012-02-29T14:32:39.846000",
                        "elements": {
                            "045e8b26-3614-49b8-97a7-a5c6ca4f112f": "[check] Boxee app library",
                            "08cf2097-daa5-4139-a8f5-686a39419da1": "[x]",
                            "0c843de7-5446-4990-8315-b643b972807b": "[p-3] Netflix, Amazon Instant Video, YouTube",
                            "1ee41dd2-eac0-4a92-8e3f-6038c4e5e42f": "[x]",
                            "41b820c4-e7bb-4d40-aff5-124283c2e0d8": "[p-5] Up to 1080p support",
                            "5c99096f-e24d-4e78-b443-37728fb65f57": "Boxee box",
                            "7c9e41ae-6454-4ffc-bf13-a6cb8694c968": "[check] Boxee browser",
                            "94bec385-c665-49e9-b43c-c6a11fcf42c8": "[x]",
                            "b895c004-2996-47a2-9128-be3e261a2221": "[check] Android, iPhone, iPad, or iPod Touch",
                            "bb86d008-57d7-4b0a-bb53-7a6544ebe88f": "Ethernet, USB, HDMI, optical audio, composite audio, 802.11 b/g/n Wi-Fi",
                            "c4fef42e-301e-4ad3-a921-d62eb65c49c4": "[p-4] Comes with a remote"
                        },
                        "id": "4f4ea787cac041000e000003"
                    },
                    {
                        "created": "2012-02-29T13:55:20.096000",
                        "elements": {
                            "045e8b26-3614-49b8-97a7-a5c6ca4f112f": "[check] Roku Channel Store",
                            "08cf2097-daa5-4139-a8f5-686a39419da1": "[x]",
                            "0c843de7-5446-4990-8315-b643b972807b": "[p-4] Netflix, Hulu Plus, Amazon Instant Video, YouTube",
                            "1ee41dd2-eac0-4a92-8e3f-6038c4e5e42f": "[x]",
                            "41b820c4-e7bb-4d40-aff5-124283c2e0d8": "[p-5] Up to 1080p support",
                            "5c99096f-e24d-4e78-b443-37728fb65f57": "Roku TV box",
                            "7c9e41ae-6454-4ffc-bf13-a6cb8694c968": "[x]",
                            "94bec385-c665-49e9-b43c-c6a11fcf42c8": "[x]",
                            "b895c004-2996-47a2-9128-be3e261a2221": "[check] iPhone, iPad, or iPod Touch",
                            "bb86d008-57d7-4b0a-bb53-7a6544ebe88f": "Ethernet, USB, HDMI, composite audio and video, Bluetooth 3.0 (for Roku game remote), Wi-Fi b/g/n",
                            "c4fef42e-301e-4ad3-a921-d62eb65c49c4": "[p-5] Comes with a Bluetooth remote with motion control for games"
                        },
                        "id": "4f4e9ec84a8422000e000002"
                    },
                    {
                        "created": "2012-02-29T12:42:07.461000",
                        "elements": {
                            "045e8b26-3614-49b8-97a7-a5c6ca4f112f": "[x] You can jailbreak it to do this, though",
                            "08cf2097-daa5-4139-a8f5-686a39419da1": "[x]",
                            "0c843de7-5446-4990-8315-b643b972807b": "[p-3] Netflix, iTunes, YouTube",
                            "1ee41dd2-eac0-4a92-8e3f-6038c4e5e42f": "[x]",
                            "41b820c4-e7bb-4d40-aff5-124283c2e0d8": "[p-3] Up to 720p support",
                            "5c99096f-e24d-4e78-b443-37728fb65f57": "Apple TV box",
                            "7c9e41ae-6454-4ffc-bf13-a6cb8694c968": "[x] You can jailbreak it and install web browser apps, though",
                            "94bec385-c665-49e9-b43c-c6a11fcf42c8": "[x]",
                            "b895c004-2996-47a2-9128-be3e261a2221": "[check] iPhone, iPad, or iPod Touch",
                            "bb86d008-57d7-4b0a-bb53-7a6544ebe88f": "Ethernet, micro-USB (for service/support only), HDMI, optical audio, 802.11n Wi-Fi",
                            "c4fef42e-301e-4ad3-a921-d62eb65c49c4": "[p-4] Comes with a mini-remote"
                        },
                        "id": "4f4e8d9f4a8422000c000003"
                    }
                ],
                "id": "4f4e8aefcac041000d000002",
                "last_modified_by_user": "2012-02-29T15:11:06.182000",
                "resource_uri": "/api/v1/grids/4f4e8aefcac041000d000002/",
                "title": "Apple TV vs. Google TV vs. Roku vs. Boxee",
                "username": "audreyr"
            },
        ],
        ...
    }