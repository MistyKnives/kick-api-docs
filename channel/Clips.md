# Clips
Get the details of a channel's clip mentioned in the URL parameters
<br>**URL**: `/api/v1/users/{username}/clips`
<br>**METHOD**: `GET`
<br>**Rate Limited?**: `YES`
<br>**Authenticated?**: `NO`

<details>
    <summary style="font-weight: bold">Response</summary>
    
```json
{
  "clips": [
    {
      "id": Integer,
      "is_mature": Boolean,
      "title": String,
      "duration": Integer,
      "thumbnail_url": String,
      "video_url": String,
      "view_count": Integer,
      "likes_count": Integer,
      "liked": Boolean,
      "created_at": String,
      "creator": {
        "id": Integer,
        "username": String,
        "slug": String,
        "profile_picture": String
      },
      "channel": {
        "id": Integer,
        "username": String,
        "slug": String,
        "profile_picture": String
      },
      "category": {
        "id": Integer,
        "name": String,
        "slug": String,
        "responsive": String,
        "banner": String
      }
    }
  ],
}
```
</details>

<details>
    <summary style="font-weight: bold">Example</summary>
    
```json
{
  "clips": [
    {
      "id": 8113,
      "is_mature": true,
      "title": "2.1M Juicer Peak Power, We in Malta Bucko!",
      "duration": 30,
      "thumbnail_url": "https://clips.kick.com/clips/2d30e092-55b7-4111-9858-aba2f6ead860-thumbnail.jpeg",
      "video_url": "https://clips.kick.com/clips/2d30e092-55b7-4111-9858-aba2f6ead860.mp4",
      "view_count": 17118,
      "likes_count": 234,
      "liked": false,
      "created_at": "2023-03-06T07:17:36.000000Z",
      "creator": {
        "id": 1432713,
        "username": "Casina",
        "slug": "casina",
        "profile_picture": null
      },
      "channel": {
        "id": 715,
        "username": "Trainwreckstv",
        "slug": "trainwreckstv",
        "profile_picture": "https://files.kick.com/images/user/723/profile_image/conversion/87a305ea-3bc8-4e65-8772-9a453e8b9f37-thumb.webp"
      },
      "category": {
        "id": 28,
        "name": "Slots & Casino",
        "slug": "slots",
        "responsive": "https://files.kick.com/images/subcategories/28/banner/fb2219e4-f490-4c73-ba3f-575ea6333f2f",
        "banner": "https://files.kick.com/images/subcategories/28/banner/fb2219e4-f490-4c73-ba3f-575ea6333f2f"
      }
    }
 ],
}
```
</details>

**Errors**:

| Error         | Response      | Reason |
| ------------- | ------------- | ------ |
| 404           | Not Found     | Account with 'username' was not found in the database. |

