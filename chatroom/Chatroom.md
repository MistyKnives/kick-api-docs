# Chatroom
Get the information for a Channel's chatroom.
**URL**: `/api/v1/{username}/chatroom`
**METHOD**: `GET`
**Rate Limited?**: `YES`
**Authenticated?**: `NO`

<details>
    <summary style="font-weight: bold">Response</summary>
    
```json
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
    "role":  String,
    "follower_badges": Array,
    "muted_users": Array,
    "can_host": Boolean,
    "chatroom": {
        "id": Integer,
        "chatable_type": String,
        "channel_id": Integer,
        "created_at": String,
        "updated_at": String,
        "chat_mode_old": String,
        "chat_mode": String,
        "slow_mode": Boolean,
        "chatable_id": Integer,
        "followers_mode": Boolean,
        "subscribers_mode": Boolean,
        "emotes_mode": Boolean,
        "message_interval": Integer,
        "following_min_duration": Integer
    },
    "emotes": [
        {
            "id": Integer,
            "channel_id": Integer,
            "name": String,
            "subscribers_only": Boolean,
            "image": String
        }
    ]
}
```
</details>

<details>
    <summary style="font-weight: bold">Example</summary>
    
```json 
{
    "id": 90876,
    "user_id": 91898,
    "slug": "averagedad",
    "is_banned": false,
    "playback_url": "https:\/\/fa723fc1b171.us-west-2.playback.live-video.net\/api\/video\/v1\/us-west-2.196233775518.channel.VpUP15HU1JrL.m3u8",
    "name_updated_at": "2023-03-15 15:56:34",
    "vod_enabled": true,
    "subscription_enabled": true,
    "cf_rate_limiter": "1.85",
    "role": null,
    "follower_badges": [],
    "muted_users": [],
    "can_host": true,
    "chatroom": {
        "id": 90874,
        "chatable_type": "App\\Models\\Channel",
        "channel_id": 90876,
        "created_at": "2022-12-06T06:49:52.000000Z",
        "updated_at": "2023-04-19T07:01:02.000000Z",
        "chat_mode_old": "public",
        "chat_mode": "public",
        "slow_mode": false,
        "chatable_id": 90876,
        "followers_mode": false,
        "subscribers_mode": false,
        "emotes_mode": false,
        "message_interval": 0,
        "following_min_duration": 10
    },
    "emotes": [
        {
            "id": 227701,
            "channel_id": 90876,
            "name": "bot",
            "subscribers_only": false,
            "image": null
        }
    ]
}
```
</details>

**Errors**:

| Error         | Response      | Reason |
| ------------- | ------------- | ------ |
| 404           | Not Found     | Account with 'username' was not found in the database. | 