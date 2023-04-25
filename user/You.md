# User
Get the details of your User object.
<br>**URL**: `/api/v1/user`
<br>**METHOD**: `GET`
<br>**Rate Limited?**: `YES`
<br>**Authenticated?**: `YES`

<h5>I'm not sure why but there's no data being responded to this endpoint. Let me know if anyone can get access to it!</h5>

<details>
    <summary style="font-weight: bold">Response</summary>

```json
{
    "id": Long,
    "email": String,
    "username": String,
    "google_id": String,
    "agreed_to_terms": Boolean,
    "email_verified_at": String,
    "bio": String,
    "country": String,
    "state": String,
    "city": String,
    "enable_live_notifications": Boolean,
    "instagram": String,
    "twitter": String,
    "youtube": String,
    "discord": String,
    "tiktok": String,
    "facebook": String,
    "enable_onscreen_live_notifications": Boolean,
    "apple_id": String,
    "email_updated_at": String,
    "country_code": String,
    "profilepic": String,
    "is_2fa_setup": Boolean,
    "redirect": String,
    "channel_can_be_updated": Boolean,
    "is_live": Boolean,
    "roles": Array,
    "streamer_channel": {
        "id": Long,
        "user_id": Long,
        "slug": String,
        "is_banned": Boolean,
        "playback_url": String,
        "name_updated_at": String,
        "vod_enabled": Boolean,
        "subscription_enabled": Boolean,
        "cf_rate_limiter": String,
        "can_host": Boolean
    }
}
```
</details>

<details>
    <summary style="font-weight: bold">Example</summary>

```json
{
    "id": 842582,
    "email": "",
    "username": "MistyKnives",
    "google_id": null,
    "agreed_to_terms": true,
    "email_verified_at": "2023-02-07T08:12:41.000000Z",
    "bio": "",
    "country": "",
    "state": "",
    "city": "",
    "enable_live_notifications": true,
    "instagram": "MistyKnives",
    "twitter": "MistyKnives",
    "youtube": "@MistyKnives",
    "discord": "",
    "tiktok": "MistyKnives",
    "facebook": "",
    "enable_onscreen_live_notifications": true,
    "apple_id": null,
    "email_updated_at": "2023-02-07T00:00:00.000000Z",
    "country_code": null,
    "profilepic": "https://files.kick.com/images/user/842582/profile_image/conversion/82d8365f-1ca8-487c-9cc4-914175f06f5a-medium.webp",
    "is_2fa_setup": true,
    "redirect": null,
    "channel_can_be_updated": true,
    "is_live": false,
    "roles": [],
    "streamer_channel": {
        "id": 815591,
        "user_id": 842582,
        "slug": "mistyknives",
        "is_banned": false,
        "playback_url": "https://fa723fc1b171.us-west-2.playback.live-video.net/api/video/v1/us-west-2.196233775518.channel.orCcYCizD63V.m3u8",
        "name_updated_at": null,
        "vod_enabled": true,
        "subscription_enabled": false,
        "cf_rate_limiter": "1.85",
        "can_host": true
    }
}
```
</details>

| Error         | Response      | Reason |
| ------------- | ------------- | ------ |
| N/A           | Not Authenicated     | You are not authenticated. | 