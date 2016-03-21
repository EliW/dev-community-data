# Community Data

[![Build Status](https://travis-ci.org/afilina/dev-community-data.svg?branch=master)](https://travis-ci.org/afilina/dev-community-data)

The goal is simple: collect all data, current and historical for anyone to use in order to make a stronger developer community.

Feel free to add your own record, fix erroneous data and add additional fields.

## User Groups

The file [/data/user-groups.json](https://github.com/afilina/dev-community-data/blob/master/data/user-groups.json) lists all user groups. Leave "last_meetup" blank if still active.

Tip: add your entry to the top of file to avoid merge conflicts.

```json
{
    "key": "example",
    "name": "Full user group name",
    "tags": ["php", "js"],
    "first_event": "yyyy-mm-dd",
    "last_event": "yyyy-mm-dd", 
    "locations": [
        {
            "name": "City, State (if applies), Country",
            "first_meetup": "yyyy-mm-dd",
            "last_meetup": "yyyy-mm-dd"
        }
    ],
    "website": "http://example.com",
    "twitter": "@twitter_handle",
    "calendar_feed": "http://example.com/feed.rss"
}
```

## Conferences

The file [/data/conferences.json](https://github.com/afilina/dev-community-data/blob/master/data/conferences.json) lists all conferences. Leave "last_event" blank if still active.

Tip: add your entry to the top of file to avoid merge conflicts.

```json
[
    {
        "key": "example",
        "name": "Full conference name",
        "tags": ["ruby"],
        "first_event": "yyyy-mm-dd",
        "last_event": "",
        "speaker_kit": {
            "ticket_included": true,
            "hotel_included": true,
            "travel_included": true
        },
        "events": [
            {
                "name": "Name of specific edition",
                "location": {
                    "name": "City, State (if applies), Country"
                },
                "event_start": "yyyy-mm-dd",
                "event_end": "yyyy-mm-dd",
                "cfp_start": "yyyy-mm-dd",
                "cfp_end": "yyyy-mm-dd",
                "session_feed": "https://example.com/2016/sessions.json",
                "speaker_feed": "https://example.com/2016/speakers.json",
                "hashtag": "#hashtag",
                "organizers": [
                    {
                        "name": "Organizer Name",
                        "twitter": "@twitter_handle"
                    }
                ]
            }
        ],
        "website": "https://example.com",
        "twitter": "@twitter_handle"
    }
]
```
