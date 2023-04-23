# Get Channel Emotes
Get a list of the emotes from a channel.
<br>**URL**: `/emotes/{channel}`
<br>**METHOD**: `GET`
<br>**Rate Limited?**: `YES`
<br>**Authenticated?**: `NO`

<details>
    <summary style="font-weight: bold">Response</summary>

```json
[
    {
        "id": Integer,
        "user_id": Integer,
        "slug": String,
        "is_banned": Boolean,
        "playback_url": String,
        "name_updated_at": String,
        "vod_enabled": Boolean,
        "subscription_enabled": Boolean,
        "cf_rate_limiter": String,
        "emotes": [
            {
                "id": Integer,
                "channel_id": Integer,
                "name": String,
                "subscribers_only": Boolean
            }
        ]
    }
]
```
</details>

<details>
    <summary style="font-weight: bold">Example</summary>

```json
[
    {
        "id": 688865,
        "user_id": 710409,
        "slug": "nay",
        "is_banned": false,
        "playback_url": "https:\/\/fa723fc1b171.us-west-2.playback.live-video.net\/api\/video\/v1\/us-west-2.196233775518.channel.XEQ4paqXEtIV.m3u8",
        "name_updated_at": null,
        "vod_enabled": true,
        "subscription_enabled": true,
        "cf_rate_limiter": "1.85",
        "emotes": [
            {
                "id": 628810,
                "channel_id": 688865,
                "name": "nayAYO",
                "subscribers_only": false
            }
        ]
    }
]
```
</details>

| Error         | Response      | Reason |
| ------------- | ------------- | ------ |
| 404           | Not Found     | Channel with the username specified not found. | 