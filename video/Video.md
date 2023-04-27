# User
Get the details of a video
<br>**URL**: `api/v1/video/{videoid}`
<br>**METHOD**: `GET`
<br>**Rate Limited?**: `YES`
<br>**Authenticated?**: `NO`


<details>
    <summary style="font-weight: bold">Response</summary>
    
```json
{
	"id": Long,
	"live_stream_id": Long,
	"slug": String,
	"thumb": String,
	"s3": String,
	"trading_platform_id": String,
	"created_at": String,
	"updated_at": String,
	"uuid": String,
	"views": Integer,
	"deleted_at": String,
	"source": String,
	"livestream": {
		"id": Long,
		"slug": String,
		"channel_id": Long,
		"created_at": String,
		"session_title": String,
		"is_live": Boolean,
		"risk_level_id": String,
		"source": String,
		"twitch_channel": String,
		"duration": Long,
		"language": String,
		"is_mature": Boolean,
		"viewer_count": Integer,
		"thumbnail": String,
		"channel": {
			"id": Long,
			"user_id": Long,
			"slug": String,
			"is_banned": Boolean,
			"playback_url": String,
			"name_updated_at": String,
			"vod_enabled": Boolean,
			"subscription_enabled": Boolean,
			"cf_rate_limiter": String,
			"followersCount": Integer,
			"user": {
				"profilepic": String,
				"bio": String,
				"twitter": String,
				"facebook": String,
				"instagram": String,
				"youtube": String,
				"discord": String,
				"tiktok": String,
				"username": String
			},
			"can_host": Boolean,
			"verified": Boolean
		},
		"categories": [{
			"id": Integer,
			"category_id": Integer,
			"name": String,
			"slug": String,
			"tags": Array,
			"description": String,
			"deleted_at": String,
			"category": {
				"id": Integer,
				"name": String,
				"slug": String,
				"icon": String
			}
		}]
	}
}
```
</details>

<details>
    <summary style="font-weight: bold">Example</summary>

```json
{
	"id": 1858666,
	"live_stream_id": 1858045,
	"slug": null,
	"thumb": null,
	"s3": null,
	"trading_platform_id": null,
	"created_at": "2023-04-26T02:01:32.000000Z",
	"updated_at": "2023-04-26T02:01:32.000000Z",
	"uuid": "e7f5ff35-3c08-45e7-8581-a08387b43013",
	"views": 0,
	"deleted_at": null,
	"source": "https:\/\/stream.kick.com\/ivs\/v1\/196233775518\/6BNqlIq3rMw1\/2023\/4\/26\/0\/55\/MiBumeRGtBX4\/media\/hls\/master.m3u8",
	"livestream": {
		"id": 1858045,
		"slug": "d3d7b-minecraft-with-friends",
		"channel_id": 1623279,
		"created_at": "2023-04-26 00:55:39",
		"session_title": "Minecraft with friends",
		"is_live": false,
		"risk_level_id": null,
		"source": null,
		"twitch_channel": null,
		"duration": 3856000,
		"language": "English",
		"is_mature": false,
		"viewer_count": 2,
		"thumbnail": null,
		"channel": {
			"id": 1623279,
			"user_id": 1671901,
			"slug": "diffusionai",
			"is_banned": false,
			"playback_url": "https:\/\/fa723fc1b171.us-west-2.playback.live-video.net\/api\/video\/v1\/us-west-2.196233775518.channel.6BNqlIq3rMw1.m3u8",
			"name_updated_at": null,
			"vod_enabled": true,
			"subscription_enabled": false,
			"cf_rate_limiter": "1.85",
			"followersCount": 9,
			"user": {
				"profilepic": "https:\/\/files.kick.com\/images\/user\/1671901\/profile_image\/4c308a84-c89b-4a48-8357-507853320f40",
				"bio": "Creating Ai Art",
				"twitter": "",
				"facebook": "",
				"instagram": "",
				"youtube": "",
				"discord": "",
				"tiktok": "",
				"username": "DiffusionAi"
			},
			"can_host": true,
			"verified": null
		},
		"categories": [{
			"id": 718,
			"category_id": 1,
			"name": "Minecraft Dungeons",
			"slug": "minecraft-dunegons",
			"tags": ["RPG", "Adventure Game"],
			"description": null,
			"deleted_at": null,
			"category": {
				"id": 1,
				"name": "Games",
				"slug": "games",
				"icon": "\ud83d\udd79\ufe0f"
			}
		}]
	}
}
```
