# Livestreams
Get livestream details of your followings
<br>**URL**: `/api/v1/user/livestreams`
<br>**METHOD**: `GET`
<br>**Rate Limited?**: `YES`
<br>**Authenticated?**: `YES`

<details>
    <summary style="font-weight: bold">Response</summary>
    
```json
[
  {
    "id": Integer,
    "slug": String,
    "channel_id": Integer,
    "created_at": String,
    "session_title": String,
    "is_live": Boolean,
    "risk_level_id": Integer,
    "source": String,
    "twitch_channel": String,
    "duration": Integer,
    "language": String,
    "is_mature": Boolean,
    "viewer_count": Integer,
    "order": Integer,
    "thumbnail": {
     "srcset": String,
      "src": String
},
    "viewers": Integer,
    "channel": {
      "id": Integer,
      "user_id": Integer,
      "slug": String,
      "is_banned": Booealn,
      "playback_url": String
      "name_updated_at": String,
      "vod_enabled": Boolean,
      "subscription_enabled": Boolean,
      "cf_rate_limiter": String,
      "can_host": Boolean,
      "user": {
        "id": Integer,
        "username": String,
        "agreed_to_terms": Boolean,
        "email_verified_at": String,
        "bio": String,
        "country": String,
        "state": String,
        "city": String,
        "instagram": String,
        "twitter": String,
        "youtube": String,
        "discord": String,
        "tiktok": String,
        "facebook": String,
        "country_code": String,
        "profilepic": String
      }
    },
    "categories": [
      {
        "id": Integer,
        "category_id": Integer,
        "name": String,
        "slug": "String,
        "tags": [
          String
        ],
        "description": String,
        "deleted_at": String,
        "category": {
          "id": Integer,
          "name": String,
          "slug": String,
          "icon": String
        }
      }
    ]
  }
```
</details>

<details>
    <summary style="font-weight: bold">Example</summary>
    
```json
[
  {
    "id": 1835603,
    "slug": "5bfd7-need-a-max-win-please",
    "channel_id": 715,
    "created_at": "2023-04-25 10:24:13",
    "session_title": "NEED A MAX WIN PLEASE",
    "is_live": true,
    "risk_level_id": null,
    "source": null,
    "twitch_channel": null,
    "duration": 0,
    "language": "English",
    "is_mature": true,
    "viewer_count": 10678,
    "order": 1,
    "thumbnail": {
      "srcset": "https://images.kick.com/video_thumbnails/p0mBRipm9p81/D31zSqjfVCoZ/1080.webp 1920w, https://images.kick.com/video_thumbnails/p0mBRipm9p81/D31zSqjfVCoZ/720.webp 1280w, https://images.kick.com/video_thumbnails/p0mBRipm9p81/D31zSqjfVCoZ/360.webp 480w, https://images.kick.com/video_thumbnails/p0mBRipm9p81/D31zSqjfVCoZ/480.webp 640w, https://images.kick.com/video_thumbnails/p0mBRipm9p81/D31zSqjfVCoZ/160.webp 284w",
      "src": "https://images.kick.com/video_thumbnails/p0mBRipm9p81/D31zSqjfVCoZ/720.webp"
    },
    "viewers": 10678,
    "channel": {
      "id": 715,
      "user_id": 723,
      "slug": "trainwreckstv",
      "is_banned": false,
      "playback_url": "https://fa723fc1b171.us-west-2.playback.live-video.net/api/video/v1/us-west-2.196233775518.channel.p0mBRipm9p81.m3u8",
      "name_updated_at": null,
      "vod_enabled": true,
      "subscription_enabled": true,
      "cf_rate_limiter": "1.55",
      "can_host": true,
      "user": {
        "id": 723,
        "username": "Trainwreckstv",
        "agreed_to_terms": true,
        "email_verified_at": "2022-10-22T11:37:42.000000Z",
        "bio": "squadW - #1 Podcast",
        "country": "",
        "state": "",
        "city": "",
        "instagram": "tylerniknam",
        "twitter": "Trainwreckstv",
        "youtube": "trainwreckstv",
        "discord": "",
        "tiktok": "",
        "facebook": "",
        "country_code": null,
        "profilepic": "https://files.kick.com/images/user/723/profile_image/conversion/87a305ea-3bc8-4e65-8772-9a453e8b9f37-thumb.webp"
      }
    },
    "categories": [
      {
        "id": 28,
        "category_id": 4,
        "name": "Slots & Casino",
        "slug": "slots",
        "tags": [
          "Gambling"
        ],
        "description": null,
        "deleted_at": null,
        "category": {
          "id": 4,
          "name": "Gambling",
          "slug": "gambling",
          "icon": "🎰"
        }
      }
    ]
  },
```
</details>

**Errors**:

| Error         | Response      | Reason |
| ------------- | ------------- | ------ |
| 401           | Unauthorized  | Unauthenticated |
